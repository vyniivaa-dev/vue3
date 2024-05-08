<template>
    <h1>Email : {{email}}</h1>
    <h1>Name : {{getName("Vue 3")}}</h1>
    <h1>Data : {{getData().email}}</h1>
</template>

<script>
    export default {
        name: 'HomePage',
        data()
        {
            return {
                email: "vue@test.com",
            }
        },
        methods: {
            getName(name)
            {
                return name;
            },
            getData()
            {
                return {
                    name: "Vue 3",
                    email: this.email
                }
            }
        }
    }
</script>

<style scoped>
h1{
    color:orange    
}
</style>