<template>
  <div class="Result">
   <p>
        Result is : {{ score }}
   </p>
   <p class="rank">
       {{ rank }}
   </p>
  </div>
</template>

<script>
export default {
    props: [ 'score' ],
    data() {
        return {
            rank: null
        }
    },    
    mounted() {
        if (this.score < 250) {
            this.rank = 'Best fingers'
        } else if (this.score < 500) {
            this.rank = 'Rapid reflexes'
        } else {
            this.rank = 'Snail pace ...'
        }
    }
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

    .rank {
        font-size: 1.4em;
        color: white;
    }
</style>