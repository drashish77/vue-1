<template>
<div class="shadow-lg m-2 px-4 py-6">

    <h3 class="font-bold text-2xl text-red-400">Title: {{title}}</h3>
    <h2 class="text-blue-400">My name is {{getName('Ashish K')}}</h2>
    <h2 class="text-green-400">My employer is {{getName('Gaurav Gupta')}}</h2>
    <h3 class=""> name: {{getData().name}} and email: {{getData().email}}</h3>
    <h3>My email is {{email}}</h3>
    <h4>my phone is {{phone}}</h4>
    
</div>
</template>

<script>
export default {
    name: 'ExampleVue',
    props: {
        title: String
    },
    data() {
        return {
            name: 'Ashish Gupta',
            email: 'Ashish@abc.com',
            phone: 10203030,
            users: [{
                    name: 'Gaurav',
                    email: 'Gaurav@gmail.com',
                    phone: 10203030
                },
                {
                    name: 'pritesh',
                    email: 'pritesh@gmail.com',
                    phone: 10203030
                },
                {
                    name: 'Timorwe',
                    email: 'Timorwe@gmail.com',
                    phone: 10203030
                },
            ]
        }
    },
    methods: {
        getName(x) {
            return x
        },
        getData() {
            return {
                name: this.name,
                email: this.email
            }
        }
    },
}
</script>
