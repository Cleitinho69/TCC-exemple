<template id="app">
    <div>
        <header>
            <nav />
            <a href="">Entrar</a>
        </header>
        <main>
            <materias />
        </main>
        <footer>
        </footer>
    </div>
</template>

<style scoped>
</style>

<style>
#app{
    width: 100%;
    height: 100%;
    display: flex;
    flex-direction: column;
    justify-content: space-between;
    align-items: center;
    background-color: green;
}
*{
    padding: 0;
    margin: 0;
    border: 0;
}
    body,html{
        width: 100vw;
        height: 100vh;
    }
</style>

<script>
    import nav from '../Components/nav.vue'
    import materias from '../Pages/materias.vue'

    export default {
        data() {
            return {
                nome_materia: 'Matemática'
            }
        },
        methods: {
            click_atividade(){
                console.log('click_atividade')
            }
        },
        components: {
            nav,
            materias
        },
    }
</script>