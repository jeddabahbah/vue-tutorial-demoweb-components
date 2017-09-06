<template>
    <div>
      <app-header></app-header>
      <app-article></app-article>
      <app-footer></app-footer>
    </div>
</template>

<script>

import Header from './components/Header.vue';
import Footer from './components/Footer.vue';
import Article from './components/Article.vue';

export default {
  components:{
    'app-header' : Header,
    'app-footer' : Footer,
    'app-article' : Article
  },
  data () {
    return {
      
    }
  }
}
</script>

<style>

</style>
