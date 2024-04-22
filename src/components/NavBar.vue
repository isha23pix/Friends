<template>
    <div class="NavBar">
     <AppName />
     <SearchBar />
     <Expense/>
     <User1/>
     <notif/>
     <!-- Add other navigation elements here -->
   </div>
 </template>
 
 <script>
  import { defineComponent } from "vue";
 import AppName from "./AppName.vue";
 import Expense from "./Expense.vue";
 import SearchBar from "./SearchBar.vue";
 import notif from "./notif.vue"
 import User1 from "./User1.vue";
   export default defineComponent({
     name: "NavBar",
     components: { AppName,Expense,SearchBar,User1,notif },
   });
 </script>
 
 <style scoped>
 @media screen and (max-width: 768px) {
   .NavBar {
    display: flex;
  align-items: center;
  justify-content: space-between;
  padding: 10px; /* Adjust padding as needed */
   }
 }
 </style>
 