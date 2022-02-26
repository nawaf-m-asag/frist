<template>
  <div class="about">
    <h1>This is an about page 2</h1>
    <welcomeMessage />
  </div>
</template>

<script>
//@ => src  
import welcomeMessage from "@/components/WelcomeMessage.vue";
export default {
  name: "about",
  components: {
    welcomeMessage,
  },
};
</script>
