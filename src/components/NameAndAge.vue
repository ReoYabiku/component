<template>
    <div class="box">
        <h1>{{name}}さん</h1>
        <h2>{{age}}歳</h2>
    </div>
</template>

<script>
export default {
  name: 'NameAndAge',
  props: {
      name: String,
      age: String
  }
}
</script>

<style scoped>
h1 {
  color: black;
}

.box{
    border: 5px dotted black;
    padding: 0 50px;
    margin: 50px 10px;
}

</style>
