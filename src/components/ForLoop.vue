<template>
<div class="m-5">
    <h1>For loop video</h1>
</div>
<ul>
    <li v-for="(item, idx) in technology" :key="idx">{{item}}</li>
</ul>
<ul>
    <li v-for="(user, idx) in users" :key="idx">{{user.name}}</li>
</ul>
</template>

<script>
export default {
    data() {
        return {
            technology: [
                'java', 'node', 'php', 'html', 'json'
            ],
            users: [{
                    name: 'ashish',
                    email: 'ashish@gmail.com'
                },
                {
                    name: 'kamal',
                    email: 'kamal@gmail.com'
                },
                {
                    name: 'rahul',
                    email: 'rahul@gmail.com'
                },
                {
                    name: 'javed',
                    email: 'javed@gmail.com'
                },
            ]
        }
    },
}
</script>
