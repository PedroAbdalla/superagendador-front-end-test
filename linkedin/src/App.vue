<template>
<div id="app">
    <div class="topo">
         <img alt="Github logo" src="./assets/shape.png">
         <b>Github</b>&nbsp;profiles
    </div>
    <!-- <div id="nav">
        <router-link to="/">Home</router-link> |
        <router-link to="/about">About</router-link>
    </div> -->
    <router-view/>
</div>
</template>

<style lang="scss">
#app {
    font-family: 'Open Sans', sans-serif;
    .topo {
        background-color: #24292e;
        padding: 6px 10px;
        color: white;
        display: flex;
        align-items: center;
        img {
            margin-right: 5px; 
        }
    }
}
#nav {
padding: 30px;
a {
    font-weight: bold;
    color: #2c3e50;
    &.router-link-exact-active {
    color: #42b983;
    }
}
}
</style>
