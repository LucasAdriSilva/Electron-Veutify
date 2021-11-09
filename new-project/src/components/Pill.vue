<template>
  <div class="pill"> 
      <Span class="name">{{name}}</Span>
      <Span class="amount">{{amount}}</Span>
  </div>
</template>

<script>
export default {
    props:['name','amount']
}
</script>

<style scoped>
    .pill{  
        margin: 10px;
        background-color: rgb(146, 146, 231);
        color: cornsilk;
        height: 55px;
        border-radius: 25px;
        font-size: 1.3rem;
        font-weight: bold;

        display: flex;
        align-items: center;
    }

    .pill .name{
        margin-left: 15px;
    }

    .pill .amount{
        margin: 10px;
        padding: 5px;
        height: 35px;
        width: 35px;
        border-radius: 18px;
        background-color: white;
        color: rgb(146, 146, 231);
        font-size: 14px;

        display: flex;
        justify-content: center;
        align-items: center;


    }

</style>