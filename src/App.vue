<!-- template > html코드 -->
<template>
  <!-- <div class="name">{{ name }}</div> -->
  <div class="name">{{ greeting(name) }}</div>
</template>


<!-- javascript코드 -->
<!-- 컴포지션 API / 옵션 API-->
<script>
  export default {
    setup(){
      const name = "HYJ_s2";
      const greeting= (name)=>{
        return 'Hello, ' + name;
      }
     return {
      name,
      greeting
     }
    }
  }

</script>


<!-- css코드 -->
<style>
  .name{
    color: gray;
    font-size: 4rem;

  }
</style>

<!-- vue2 vs vue3
> vue2 : template 안에서 div 하나로 전체를 감싸줌(프레그먼트같은 개념인듯.) >>> vue3에서는 안써도됨
>  

-->