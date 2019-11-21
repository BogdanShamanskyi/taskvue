<template>
    <li 
        class="list-group-item alert alert-warning alert-dismissible fade show mb-2"
        role="alert"
        v-if="!checked ? true : !checked"
        >

        {{'First task'}}

        <label 
            aria-label="Close" 
            class="close mr-4" 
            data-dismiss="alert"
            >

            <input 
                aria-label="Checkbox for following text input" 
                type="checkbox" 
                v-model="checked"
                >

            <span aria-hidden="true" class="mr-4"></span>

        </label>

        <button 
            type="button"
            @click="destroyTask" 
            v-if="checked"
            class="close" 
            aria-label="Close"
            data-dismiss="alert"
            >

            <span aria-hidden="true">&times;</span>

        </button>
    </li>
</template>

<script>
    export default {
        name: "Task",
        data: () => ({
            checked: false
        })
    }
</script>