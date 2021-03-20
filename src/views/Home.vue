<template>
  <div id="home">
    <input type="text" v-model="childText" />
    <button @click="sendParent">自動住所検索</button>
  </div>
</template>

<script>

export default {
  data() {
    return {
      childtext: ""
    };
  },
  

  methods: {
    sendParent() {
      this.$emit("getChildText", this.childText);
    }
  }
};
</script>
















