<template>
  <h1>{{ msg }}</h1>
  <ParentComponent>
    <ChildComponent style="background-color: aqua" />
  </ParentComponent>
</template>

<script setup lang="ts">
import { ref } from "vue";
import { ParentComponent, ChildComponent } from "vue-broken-hmr-lib";
defineProps<{ msg: string }>();

const count = ref(0);
</script>
<style>
.white {
  color: white;
}
</style>
