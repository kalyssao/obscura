<template>
    <div class="search">
        <form @submit="search" class="search_form">
            <input
                v-model="searchTerm"
                type="text"
                class="search_form_field"
                placeholder="Enter term here"
            />
        </form>
        <div v-if="loading" class="signal"></div>
    </div>
</template>

<script>
export default {
  name: 'RwvSearch',
  data() {
    return {
      loading: false,
      searchTerm: '',
    };
  },
  methods: {
    search() {
      console.log('searching...');
    },
  },
};
</script>

<style>
.search {
    width: 100%;
    height: 100%;
    position: relative;
    animation-duration: 0.5s;
}
.search_form{
    color: white;
    background-color: rgb(65, 65, 65);
    border-radius: 500px;
    display: flex;
    margin: 0 auto;
    align-items: center;
    padding-left: 30px;
    transition: all 0.3s;
}
.search_form_field {
    background: none;
    border: none;
    padding: 8px 0;
    font-size: 17px;
    width: 500px;
    transition: all 0.3s;
}
.search_form_field:focus-wthin {
    width: 400px;
    border: none;
}

</style>
