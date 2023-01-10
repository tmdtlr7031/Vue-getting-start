<template>
  <!-- 최상위 요소는 하나만 있어야함 (같은 레벨로 복수개 불가)-->
  <div>
    <app-header 
      v-bind:prosdata="str"
      v-on:renew="renewStr"></app-header>
  </div>
</template>

<script>
import AppHeader from './components/AppHeader.vue';

export default {
  data: function() {
    return {
      str : 'Header'
    }
  },
  components: {
    'app-header' : AppHeader
  },
  methods: {
    renewStr : function() {
      this.str = 'hi';
    }
  }
}
</script>

<style>

</style>