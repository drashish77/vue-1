<template>
<!-- <h1 v-on:mousemove="onMouseMoved()">
    This is an event page
</h1> -->
<h3>count: {{count}}</h3>
<!-- <button @click="increment" class="bg-gray-500 px-2 text-white text-2xl">⬆️ Count</button>
<button @click="decrement" class="bg-gray-500 px-2 text-white text-2xl">⬇️ Count</button> -->

<input type="text" class="px-2 py-4 border" v-model="input">
<h3>Input: {{input}}</h3>
</template>

<script>
export default {
    name: 'Event-vue',
    data() {
        return {
            count: 0,
            input: 'Enter ur text'
        }
    },
    methods: {
        increment() {
            this.count += 1
        },
        decrement() {
            this.count -= 1
        }
    },
}
</script>
