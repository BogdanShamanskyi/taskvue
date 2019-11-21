<template>
    <div class="jumbotron p-4">
        <div class="input-group">

            <input
                v-model="text"
                type="text"
                class="form-control mb-2" 
                placeholder="Add task"
                aria-describedby="basic-addon2"
                >

            <button @click="some-event" class="btn btn-primary ml-2">Add</button>

        </div>

        <div class="custom-control custom-checkbox mr-sm-2">

            <input 
                type="checkbox"
                class="custom-control-input"
                id="customControlAutosizing"
                >

            <label 
                class="custom-control-label"
                for="customControlAutosizing"
                >

                All tasks

            </label>
        </div>
    </div>
</template>

<script>
    export default {
        name: "InputGroup"
    }
</script>