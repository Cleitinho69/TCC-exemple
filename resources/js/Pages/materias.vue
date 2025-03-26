<template>
    <div>
        <h1>Materias</h1>
        <section id="materias">
            <materia @click_atividade="materia" :nome="nome_materia"/>
        </section>
    </div>
</template>

<script>
    export default{
        name: 'materias',
        data() {
            return {
                nome_materia: 'MATEMÁTICA'
            }
        },
        components: {
            materia: () => import('../Components/materia.vue'),
        },

    }
</script>

<style lang="css" scoped>
    #materias{
        display: flex;
        justify-content: space-around;
        align-items: center;
        flex-wrap: wrap;
    }
</style>