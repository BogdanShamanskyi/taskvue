<template>
  <div id="app" class="container">
    <h1 class="text-center">Tasks List</h1>

    <input-group class="mt-3"/>

    <tasks/>
  </div>
</template>

<script>
  import InputGroup from "./components/InputGroup";
  import Tasks from "./components/Tasks";

  export default {
    name: 'app',
    components: {
      InputGroup,
      Tasks
    }
  }
</script>

<style>
  #app {
    width: 700px;
    margin-top: 0.3em;
  }
</style>
