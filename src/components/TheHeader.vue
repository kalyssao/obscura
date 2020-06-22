<template>
    <nav class="navbar navbar-light">
        <div class="container">
            <router-link class="navbar-brand text-left" :to="{ name: 'home' }">
                <h2> obscura. </h2>
            </router-link>
            <p> A dictionary of obscure emotions. </p>
        </div>
    </nav>
</template>

<script>
export default {
  name: 'RwvHeader',
};
</script>

<style>

</style>
