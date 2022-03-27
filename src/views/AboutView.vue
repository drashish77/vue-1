<template>
<div class="about">
    <h1>This is an about page</h1>
    <ConditionalS />
    <ForLoop />
    <!-- <Child /> -->
</div>
</template>

<script>
import ConditionalS from '@/components/ConditionalS.vue'
import ForLoop from '@/components/ForLoop.vue'
// import Child from '@/components/ChildComp.vue'

export default {

    components: {
        ConditionalS,
        ForLoop,
        // Child
    }
}
</script>
