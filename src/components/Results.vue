<template>
  <div class="Result">
      Result is : {{ score }}
  </div>
</template>

<script>
export default {
    props: [ 'score' ]
}
</script>

<style>
    .Result {
        width: 500px;
        border-radius: 20px;
        background: cornflowerblue;
        color: white;
        text-align: center;
        padding: 50px 0;
        margin: 50px auto;
    }
</style>