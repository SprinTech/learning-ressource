<template>
  <ul></ul>
</template>

<script>
export default {
  data() {
    return {
      storedRessources: [
        {
          id: "official-guide",
          title: "Official Guide",
          description: "The official Vue.js documentation.",
          link: "https://vuejs.org",
        },
        {
          id: "google",
          title: "Google",
          description: "Learning to google...",
          link: "https://google.org",
        },
      ],
    };
  },
};
</script>
