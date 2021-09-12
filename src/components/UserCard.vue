<template>
<div class="rounded shadow-lg">

  <div class="flex content-center justify-center">
    <img :src="data.picture.large" class="rounded-full">
  </div>
<div class="content-center">

  <h2 class="text-center">{{data.name.last}}</h2>
</div>
  


</div>

  
</template>

<script>
export default {
name:"UserCard",
props:{
    data: {}
}
};
</script>

<style>

</style>