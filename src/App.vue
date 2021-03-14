<template>
  <div id="app">
    <sidebar id="sidebar" />
    <router-view id="router" :key="$route.path" />
  </div>
</template>
<script lang="ts">
import { defineComponent } from "vue";
import sidebar from "@/views/Sidebar.vue";
export default defineComponent({
  components: { sidebar }
});
</script>

<style>
#app {
  margin-top: 30px;
  display: flex;
}

#sidebar {
  width: 300px;
  border: 1px solid red;
  padding: 10px;
}

#router {
  flex: 1;
  border: 1px solid red;
  padding: 10px;
}
</style>
