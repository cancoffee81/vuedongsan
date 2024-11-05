<template>

    <nav class="menu">
        <a href="#" v-for="i in menu" :key="i">{{ i }}</a>
    </nav>    
    <div v-for="(prd,i) in products" :key="i">
        <h4>{{ prd }}</h4>
        <p>{{ price[i] }} 만원</p>
    </div>
</template>

<script>

export default {
  name: 'App',
  components: {
  },
  data() {
    return {
        products : ['역삼동 원룸', '천호동 원룸', '마포구 원룸'],
        price : [50, 60, 70],
        menu : ["Home", "Procudts", "About"],
    }
  }
}
</script>

<style>
.menu { background: #006; padding:15px; border-radius: 5px; text-align:center; }
.menu a { color:#fff; padding:10px; text-decoration: none; }
</style> 
