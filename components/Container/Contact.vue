<template>
  <UiContainer>
    <div class="flex flex-col items-center justify-center p-4 sm:p-8">
      <h2
        class="border-b-4 border-primary/90 text-2xl font-semibold uppercase tracking-wider sm:text-3xl lg:text-4xl"
      >
        Contact
      </h2>
      <p class="pt-4 text-center text-base tracking-wider sm:pt-6 sm:text-lg lg:text-xl">
        If you have any questions or would like to get in touch, feel free to reach out by
        submitting the form below.
      </p>

      <UiCard
        class="mt-8 w-full max-w-sm sm:max-w-md lg:max-w-lg"
        title="Send me an Email"
        description=""
      >
        <form @submit.prevent="submit">
          <UiCardContent>
            <fieldset>
              <UiVeeInput
                name="name"
                label="Name"
                placeholder="Enter your name"
                :disabled="isSubmitting"
                class="mb-2 text-sm sm:text-base"
              />
              <UiVeeInput
                name="email"
                label="Email"
                placeholder="Enter your email"
                type="email"
                :disabled="isSubmitting"
                class="mb-2 text-sm sm:text-base"
              />
              <UiVeeTextarea
                name="message"
                label="Message"
                placeholder="Enter your message"
                :disabled="isSubmitting"
                :rows="8"
                class="text-sm sm:text-base"
              />
            </fieldset>
          </UiCardContent>
          <UiCardFooter>
            <UiButton type="submit" :disabled="isSubmitting">Submit</UiButton>
          </UiCardFooter>
        </form>
      </UiCard>
    </div>
  </UiContainer>
</template>

<script lang="ts" setup>
  import emailjs from "emailjs-com";
  import { useForm } from "vee-validate";
  import { object, string } from "yup";

  const regex = /^[^<@#`'"%;\\\[\]{}|&$*^~:/!+=\r\n]*$/;

  const toast = useToast();

  const EmailSchema = object({
    name: string()
      .required()
      .label("Name")
      .max(128)
      .matches(regex, "Name contains invalid characters"),
    email: string().email().required().label("Email"),
    message: string()
      .max(500)
      .label("Message")
      .matches(regex, "Message contains invalid characters"),
  });

  const { handleSubmit, isSubmitting, resetForm } = useForm({
    validationSchema: toTypedSchema(EmailSchema),
  });

  const submit = handleSubmit(async (values) => {
    try {
      await emailjs.send(
        "service_octd1e7",
        "template_ihop6sv",
        {
          name: values.name,
          email: values.email,
          message: values.message,
        },
        "fDxD5uS1l0zCezgwT"
      );
      toast.toast({
        title: "Message Sent",
        description: "Your message has been sent successfully.",
        variant: "success",
        icon: "lucide:badge-check",
      });

      resetForm();
    } catch (error) {
      toast.toast({
        title: "Error",
        description: "Failed to send your message. Please try again later.",
        variant: "warning",
        icon: "lucide:circle-alert",
      });
    }
  });
</script>
