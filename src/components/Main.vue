<template class="main">
  <v-toolbar color="primary">
    <v-toolbar-title> Лабораторна робота №2 </v-toolbar-title>

    <v-spacer></v-spacer>

    <template v-slot:extension>
      <v-tabs v-model="tab" fixed-tabs color="secondary">
        <v-tab value="one">Завдання №1</v-tab>
        <v-tab value="two">Завдання №2</v-tab>
        <v-tab value="three">Завдання №3</v-tab>
        <v-tab value="four">Завдання №4</v-tab>
      </v-tabs>
    </template>
  </v-toolbar>

  <v-window v-model="tab" class="text-center">
    <v-window-item value="one">
      <Task1 />
    </v-window-item>

    <v-window-item value="two">
      <Task2 />
    </v-window-item>

    <v-window-item value="three">
      <Task3 />
    </v-window-item>

    <v-window-item value="four" id="calc">
      <Task4 />
    </v-window-item>
  </v-window>
</template>

<style scoped>

.v-window-item {
  height: 80vh;
}
#calc {
  display: flex;
  justify-content: center;
  height: auto;
}
</style>

<script>
import Task1 from "@/components/Task1.vue";
import Task2 from "@/components/Task2.vue";
import Task3 from "@/components/Task3.vue";
import Task4 from "@/components/Task4.vue";

export default {
  data: () => ({
    tab: null,
  }),
  components: {
    Task1,
    Task2,
    Task3,
    Task4,
  },
};
</script>