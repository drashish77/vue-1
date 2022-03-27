<template>
<div class="flex space-x-5 p-2 bg-green-200">
    <li class="px-4 py-2 bg-white">user:{{user.name}}</li>
    <li class="px-4 py-2 bg-white">user:{{user.email}}</li>
</div>
</template>

<script>
export default {
    props: {
        user: {}
    },
}
</script>
