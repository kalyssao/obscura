<template>
    <div id="app">
        <div class="container">
            <RwvHeader/>
            <div class='gradient'></div>
            <RwvMain/>
            <RwvFooter/>
        </div>
    </div>
</template>

<script>
import RwvHeader from '@/components/TheHeader.vue';
import RwvMain from '@/components/MainContent.vue';
import RwvFooter from '@/components/TheFooter.vue';

export default {
  name: 'App',
  components: {
    RwvHeader,
    RwvFooter,
    RwvMain,
  },
};

</script>

<style>
#app {
  font-family: Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
}
/*.container {
    height: 100vh;
    width: 100%;
    display: grid;
}*/
.gradient {
    color: black;
}
.main {
    position: relative;
    grid-area: 2 / 3 / 3 / 4;
    background: #232323;
    overflow-y: scroll;
    overflow-x: hidden;
    padding: 30px 40px;
    scrollbar-color: #c9c9c9 #303030;
    scrollbar-width: thin;
}
</style>
