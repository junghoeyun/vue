<script>
export default {
  data() {
    return {
      count: 0,
      titleClass: "title",
    };
  },
  methods: {
    increment() {
      this.count++;
    },
  },
};
</script>

<template>
  <h1 :class="titleClass">5</h1>
  <p>vue로 확인하는 웹페이지 입니다. 아래 버튼을 누르면 값이 1씩 증가합니다.</p>
  <button @click="increment">
    {{ count ? count : "+1" }}
  </button>
</template>

<style scoped>
.title {
  color: red;
}
</style>