<template>
  <div class="item">
    <p>todo: {{todo}}</p>
  </div>
</template>

<script>
export default {
  name: 'TodoItem',
  props: {
    todo: String,
    id: Number
  }
}
</script>

<style></style>