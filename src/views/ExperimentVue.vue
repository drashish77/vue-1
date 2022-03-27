<template>
<div class="about">
    <h1 class="text-2xl">This is an experiment page</h1>
    <Child :surname="surname" :user="user" :getData="getData" />
    <ListComp />
</div>
</template>

<script>
import Child from '@/components/ChildComp.vue'
import ListComp from '@/components/ListComp.vue'

export default {
    components: {
        Child,
        ListComp,
    },
    data() {
        return {
            surname: 'Ramesh',
            user: {
                name: 'Kamlesh',
                email: 'ramesh@gmail.com',
                phone: '123'
            }
        }
    },
    methods: {
        getData() {
            alert('Function called')
        }
    },
}
</script>
