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