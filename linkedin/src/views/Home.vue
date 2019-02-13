<template>
  <div class="home">
    <div class="row">
        <QuadroPerfil />
        <MenusRepos />
    </div>
    <!-- <img alt="Vue logo" src="../assets/logo.png">
    <HelloWorld msg="Welcome to Your Vue.js App"/> -->
  </div>
</template>
<style lang="scss">
    .row {
        margin: 0px;
    }    
</style>

<script>
// @ is an alias to /src
import HelloWorld from '@/components/HelloWorld.vue';
import QuadroPerfil from '@/components/QuadroPerfil.vue';
import MenusRepos from '@/components/MenusRepos.vue';

export default {
name: 'home',
    components: {
        HelloWorld,
        QuadroPerfil,
        MenusRepos,
    },
};
</script>
