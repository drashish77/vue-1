<template>
<div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
        <HelloWorld msg="Welcome to Your Vue.js App" />
    <div class="flex justify-center items-center flex-wrap">
        <ExampleVue title="Love you jindagi" />
        <ExampleVue title="Maje karo" />
        <ExampleVue title="Had kardi aapne" />
        <ExampleVue title="kya kar rahi ho bhai" />
    </div>
</div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import ExampleVue from '@/components/ExampleVue.vue'

export default {
    name: 'HomeView',
    components: {
        HelloWorld,
        ExampleVue,
    }
}
</script>
