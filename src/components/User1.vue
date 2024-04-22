<template>


<div :class="user">

<img :class="userChild" alt="" src="/ellipse-3@2x.png" />
 
<div :class="johnDoe">John Doe</div>

</div>
</template>
<script>
import { defineComponent } from "vue";

export default defineComponent({
name: "UserComponent1",
data() {
 return {

   user: "user",
   userChild: "userChild",
   johnDoe: "johnDoe"
 };
}
});
</script>
<style scoped>


.uppercase {
text-transform: none;
border: 2px;
}


.userChild {
width: 50px;
position: relative;
border-radius: 50%;
height: 50px;
object-fit: cover;
}

.johnDoe {
position: relative;
}

.user {
position: absolute;
top: 15px;
/* left: 1500px; */
right: 20px;
display: flex;
flex-direction: row;
align-items: center;
justify-content: center;
gap: var(--gap-9xl);
text-align: left;
font-size: var(--font-size-6xl);
color: var(--color-black);
font-family: var(--font-radley);
}

.icon {
color:#673ab7;
}

@media only screen and (max-width: 600px) {

.user{
/* left:340px; */
/* position: absolute; */
right: -96px;
}
.johnDoe{
  visibility: hidden;
}
}
@media only screen and (max-width: 419px) {

.user{
/* left:340px; */
/* position: absolute; */
right: -120px;
}
.johnDoe{
  visibility: hidden;
}
}


</style>
