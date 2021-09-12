<template>
  <div class="text-center">
      user list from api      
  </div>


<div class="flex flex-wrap content-center justify-center w-full px-32">
  <div v-for="result in data.results"
  :key="result.id" class="px-3 w-1/3 py-5">

  <UserCard :data="result" class="content-center justify-center" />
  </div>


</div>


  
</template>

<script>
import UserCard from './UserCard.vue'
export default {
  name: 'Userlist',
  components: {
      UserCard,
  },
data() {
    return {
      data: {}
    }
  },
beforeMount() {
    this.getUserLists();
  },
methods: {
   
  async getUserLists(){
      const res =  await fetch('https://randomuser.me/api?results=18');
      const data = await res.json();
      this.data = data;
   }   
}
};


</script>

<style>

</style>