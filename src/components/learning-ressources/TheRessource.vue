<template>
  <base-card>
    <base-button @click="setSelectedTab('stored-ressources')"
      >Stored Ressources</base-button
    >
    <base-button @click="setSelectedTab('add-ressource')"
      >Add Ressource</base-button
    >
  </base-card>
  <component :is="selectedTab"></component>
</template>

<script>
import StoredRessources from "./components/learning-ressources/StoredRessources.vue";
import AddRessources from "./components/learning-ressources/AddRessources.vue";

export default {
  components: {
    StoredRessources,
    AddRessources,
  },
  data() {
    return {
      selectedTab: "stored-ressources",
    };
  },
  methods: {
    setSelectedTab(tab) {
      this.selectedTab = tab;
    },
  },
};
</script>
