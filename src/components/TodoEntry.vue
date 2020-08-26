<template>
  <div class="todo-entry">
    <input type="text" placeholder="What needs to be done?" />
  </div>
</template>

<script>
export default {
  name: 'TodoEntry',
}
</script>

<style scoped>

.todo-entry {
  --placeholder-color: rgba(127,127,127,0.4);
}

input[type=text] {
  padding: 1em 6em 1em 2em;
  margin-bottom: 60px;
  text-align: left;
  color: black;
  font-size: 20px;

  border: none;

  -webkit-box-shadow: 0px 10px 50px 2px rgba(0,0,0,0.5);
  -moz-box-shadow: 0px 10px 50px 2px rgba(0,0,0,0.5);
  box-shadow: 0px 10px 50px 2px rgba(0,0,0,0.5);
}

/* Chrome, Firefox, Opera, Safari 10.1+ */
::placeholder { 
  font-style: italic;
  color: var(--placeholder-color);
}

/* Internet Explorer 10-11 */
:-ms-input-placeholder { 
  font-style: italic;
  color: var(--placeholder-color);
}

/* Microsoft Edge */
::-ms-input-placeholder { 
  font-style: italic;
  color: var(--placeholder-color);
}
</style>