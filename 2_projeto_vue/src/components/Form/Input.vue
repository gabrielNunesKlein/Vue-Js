<template>
    <div>
        <div>
            <input type="text">
        </div>
        <div>
            <input type="text">
        </div>
        <div>
            <Submit />
        </div>
    </div>
</template>

<script>
import Submit from './Submit.vue';
    export default {
        name: 'Input',
        components: {
            Submit
        }
    }
</script>
