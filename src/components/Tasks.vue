<template>
    <ol class="list-group">
        <task/>
    </ol>
</template>

<script>
    import Task from "./Task";

    export default {
        name: "Tasks",
        components: {
            Task
        }
    }
</script>