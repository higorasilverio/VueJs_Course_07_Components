<template>
    <div class="counter">
        <span>{{ counter }}</span>
        <button @click="adc">+</button>
        <button @click="subs">-</button>
    </div>
</template>

<script>
export default {
    data() {
        return {
            counter: 0
        }
    },
    methods: {
        adc() {
            this.counter++
        },
        subs() {
            this.counter--
        }
    }
}
</script>

<style>
    .counter span {
        border-bottom: 1px solid #CCC;
        height: 30px;
        padding: 5px 25px;
    }

    .counter button {
        height: 30px;
        width: 30px;
        border-radius: 15px;
        background-color: coral;
        color: #FFF;
        margin-left: 10px;
        outline: none;
    }
</style>