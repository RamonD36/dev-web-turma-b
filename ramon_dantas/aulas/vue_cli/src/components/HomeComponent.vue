<template>
  <div>
    <footer>
        <p>Bem Vindo! {{ nome }} Olá Mundo do Vue</p>
    </footer>
  </div>
</template>



<script>

    export default {
        name: 'HomeComponent',
        data() {
            return {
                nome: 'Ramon'
            }
        },

        components: {
        }

    }
</script>

<style>
</style>