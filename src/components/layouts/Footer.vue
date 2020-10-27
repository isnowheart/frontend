<template lang="pug">
  footer.footer
    span Copyright #[b C-Lab] © 2020
</template>

<script>
export default {
  name: 'Footer'
}
</script>

<style scoped>
  .footer {
    grid-area: footer;
    background-color: #DDD;
    color: #333;

    display: flex;
    align-items: center;
    justify-content: flex-end;
    padding-right: 10px;
  }
</style>