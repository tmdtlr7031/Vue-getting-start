<template>
  <!-- 최상위 요소는 하나만 있어야함 (같은 레벨로 복수개 불가)-->
  <div>
    {{ str }}
  </div>
</template>

<script>
export default {
  data: function() {
    return {
      str : 'hi'
    }
  }
}
</script>

<style>

</style>