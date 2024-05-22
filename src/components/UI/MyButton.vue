<template>
  <button class="btn"><slot></slot></button>
</template>

<script>
export default {
  name: "my-button",
};
</script>

<style scoped>
.btn {
  display: flex;
  padding: 10px 30px;
  background: none;
  color: teal;
  border: 1px solid teal;
}
</style>
