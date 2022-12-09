<template>
    <header>
        <h1>
            {{title}}
        </h1>
        <ButtonVue text="Add Task" color="green"></ButtonVue>
    
    </header> 
</template>

<script>
import ButtonVue from './Button.vue';
    export default {
        name: 'HeaderComponent',
        props : {
            "title" : String
        },
        components : {
            ButtonVue
        }
    }
</script>

<style scoped>
header{
    display: flex;
    justify-content: space-between;
    align-items: center;
    margin-bottom: 20px;
}
</style>
