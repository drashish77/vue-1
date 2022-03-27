<template>
<div>
    <input type="text" v-model="email" class="p-2 border">
    <input type="password" v-model="password" class="p-2 border">
</div>
<button @click="getData" class="border px-4 py-2 mt-5 bg-gray-600 text-white rounded">Submit</button>
<!-- <h2 class="text-blue-600">
    my name is <strong>{{myname}}</strong> and email is <strong>{{email}}</strong>
</h2> -->
<div class="">
    <h2>Technology</h2>
    <label for="java">Java</label>
    <input type="checkbox" name="java" value="java" v-model="technology" class="m-2">
    <label for="node">node</label>
    <input type="checkbox" name="node" value="node" v-model="technology" class="m-2">
    <label for="go">go</label>
    <input type="checkbox" name="go" value="go" v-model="technology" class="m-2">
    <label for="php">php</label>
    <input type="checkbox" name="php" value="php" v-model="technology" class="m-2">
</div>
<h3>Technology: {{technology}} </h3>
</template>

<script>
export default {
    data() {
        return {
            email: '',
            password: '',
            technology: []
        }
    },
    methods: {
        getData() {
            console.log('btn clicked', this.email, this.password)
        }
    },
}
</script>
