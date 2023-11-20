<template>
    <div>
        <button @click="showChild = !showChild">Show Child</button>
        <child></child>
    </div>
</template>

<script>
import Child from './Child.vue'

    export default {
        name: 'Parent',
        data(){
            return{
                showChild: true
            }
        },
        components:{
            Child
        },
        beforeCreate(){
            console.log('Parent beforeCreate')
        },
        created(){
            console.log('Parent Created')
        },
        beforeMount(){
            console.log('Parent beforeMount')
        },
        mounted(){
            console.log('Parent mounted')
        },
        beforeUpdate(){
            console.log('Parent beforeUpdate')
        },
        updated(){
            console.log('Parent updated')
        },
        beforeUnmount(){
            console.log('Parent beforeUnmount')
        },
        unmounted(){
            console.log('Parent unmounted')
        }
    }
</script>

<style scoped>

</style>