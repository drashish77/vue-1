<template>
<div>
    <h1>This is a child component</h1>
    <p>Surname: {{surname}} </p>
    <div class="">
        <h1>Users Data</h1>
        <p>name: {{user.name}}</p>
        <p>email: {{user.email}}</p>
        <p>phone: {{user.phone}}</p>
    </div>
    <button @click="getData" class="p-2 bg-green-400">Click me</button>
</div>
</template>

<script>
export default {
    props: {
        surname: String,
        user: {},
        getData: Function
    },
}
</script>

<style>

</style>
