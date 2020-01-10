<script>
export default {
    name: 'FlashCard',
    props: {
        sideA: {
            type: String,
            required: true
        },
        sideB: {
            type: String,
            required: true
        },
    },
    data() {
        return {
            showSideA: true
        };
    },
    methods: {
        flipCard() {
            this.showSideA = !this.showSideA;
        }
    }
}
</script>

<template>
    <div class='card' style='width: 500px; height: 300px' v-on:click="flipCard()">
        <div class='card-body d-flex justify-content-center align-items-center'>
            <p class='card-text align-middle'>{{this.showSideA ? sideA : sideB}}</p>
        </div>
    </div>
</template>