<template>
    <div class="materia" @click="$emit('click_atividade')"> {{ nome }} </div>
</template>

<script>
    export default{
        name: 'materia',
        emits: ['click_atividade'],
        props: {
            nome: String
        }

    }
</script>

<style>
    .materia{
        background-color: #f0f0f0;
        width: 300px;
        height: 100px;
        border-radius: 5px;
        padding: 10px;
        margin: 5px;
        cursor: pointer;
    }
</style>