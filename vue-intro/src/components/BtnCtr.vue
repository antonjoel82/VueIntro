<script>
export default {
    name: 'BtnCtr',
    props: {
        startingVal: {
            type: Number,
            required: false,
            default: 0
        }
    },
    data() {
        return {
            count: this.startingVal
        };
    },
    methods: {
        // incr() {
        //     this.count++;
        // }
    }
}
</script>

<template>
    <button v-on:click="() => count++">You clicked me {{ count }} times.</button>
</template>