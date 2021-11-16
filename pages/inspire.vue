
<template>
<div>

 <v-img :src="require('assets/img/indexWorld.png')"  />


<v-lazy>
  <v-img :src="require('assets/img/central.jpg')"  />
   
  
</v-lazy>
</div>

</template>


<script>


export default {
layout:'web',
}
</script>
