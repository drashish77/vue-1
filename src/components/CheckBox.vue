<template>
<div>
    <div>Checked names: {{ checkedNames }}</div>
    <div>profession: {{ profession }}</div>

    <input type="checkbox" id="jack" value="Jack" v-model="checkedNames">
    <label for="jack">Jack</label>

    <input type="checkbox" id="john" value="John" v-model="checkedNames">
    <label for="john">John</label>

    <input type="checkbox" id="mike" value="Mike" v-model="checkedNames">
    <label for="mike">Mike</label>
</div>
<div class="">
    <h1>Profession</h1>
    <label for="student">Student</label>
    <input type="radio" value="student" id="student" v-model="profession" name="profession">
    <label for="developer">Developer</label>
    <input type="radio" value="developer" id="developer" v-model="profession" name="profession">
</div>
</template>

<script>
export default {
    data() {
        return {
            checkedNames: [],
            profession: null
        }
    }
}
</script>
