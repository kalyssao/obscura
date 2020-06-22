<template>
    <div>
        <div v-show="loading" class="signal"></div>\
        <div :hidden="loading" class="entries fadeIn">
            <ul class="entries">
                <li class="item" v-for="entry in entries" :key="entry.entry">
            </ul>
        </div>
    </div>
</template>

<script>
export default {
  data() {
    return {
      loading: false,
      entries: [],
    };
  },
  methods: {
    init() {
      this.entries = ['sonder', 'dikjstra'];
    },
  },
  mounted() {
    this.init();
  },
};
</script>
