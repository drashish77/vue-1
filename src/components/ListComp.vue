<template>
<p>list</p>
<div>
    <ul>
        <div v-for="(item, index) in users" :key="index">
           
            <ListChild :user="item" />
        </div>
    </ul>
</div>
</template>

<script>
import ListChild from './ListChild.vue'
export default {
    components: {
        ListChild,
    },
    data() {
        return {
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
}
</script>
