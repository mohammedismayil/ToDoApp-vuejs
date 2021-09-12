<template>
  <div>

      user list from api

      
  </div>

  <li 
  v-for="result in data.results"
  :key="result.id"
  >
    <UserCard :data="result"/>
  </li>

  
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
      const res =  await fetch('https://randomuser.me/api?results=5');
      const data = await res.json();
      this.data = data;
   }   
}
};


</script>

<style>

</style>