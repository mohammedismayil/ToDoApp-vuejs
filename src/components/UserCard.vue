<template>
<div class="rounded shadow-lg bg-purple-100">
  <div class="-my-10">
     <div class="flex content-center justify-center">
      <img :src="data.picture.large" class="rounded-full ">
     </div>
     <div class="content-center">
     <h2 class="text-center">{{data.name.last}}</h2>
     </div>
     <div class="text-center">
     <h2>CEO,co-founder</h2>
      </div>
      <div class="mx-10 content-center justify-center">
       <h2>Dont be scared of the truth because we need to restart the human foundation in truth and i love you kanye west</h2>
       </div> 
       <div class="icon flex content-center justify-center">
         <img class="w-10 h-10" src="https://img.icons8.com/color/48/000000/twitter-circled--v1.png "/>
         <img class="w-10 h-10" src="https://img.icons8.com/small/96/000000/instagram-new.png"/>
         </div>     
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