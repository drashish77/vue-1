<template>
<div>
    <h1 class="text-red-500" v-if="show">Here, we are discussing conditions</h1>
    <h2 class="text-blue-500" v-else>we will discuss something else</h2>
</div>
<button @click="show=!show">Click me</button>
</template>

<script>
export default {
    data() {
        return {
            show: true
        }
    },
}
</script>
