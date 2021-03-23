<template>
  <div id="app">
    <button @click="openAccordion">アコーディオン</button>
    <div id="overlay" v-if="show">
      <div id="content">
        <p>アコーディオンの中身が入ります</p>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      show: false
    };
  },
  methods: {
    openAccordion() {
      this.show = true;
    },
    closeAccordion() {
      this.show = false;
    }
  }
}
</script>

<style>
button {
  width: 50%;
  height: 70px;
  background-color: gray;
  font-size: 20px;
  text-align: left;
}

#content p {
   
}
</style>