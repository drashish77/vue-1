<template>
<div class="home">
    <!-- <img alt="Vue logo" src="../assets/logo.png"> -->
    <HelloWorld msg="Welcome to Your Vue.js App" />
    <div class="flex justify-center items-center flex-wrap">
        <ExampleVue title="Love you jindagi" />
        <!-- <ExampleVue title="Maje karo" />
        <ExampleVue title="Had kardi aapne" />
        <ExampleVue title="kya kar rahi ho bhai" /> -->
    </div>
    <EventsView />
    <InputType />
    <CheckBox/>
</div>
</template>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue'
import ExampleVue from '@/components/ExampleVue.vue'
import EventsView from '@/components/EventsVue.vue'
import InputType from '@/components/InputType.vue'
import CheckBox from '@/components/CheckBox.vue'


export default {
    name: 'HomeView',
    components: {
        HelloWorld,
        ExampleVue,
        EventsView,
        InputType,
        CheckBox
    }
}
</script>
