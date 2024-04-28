<template>
  <div class="container">
    <h1>Custom button</h1>
    <div class="container-primary">
      <div class="primary-button" 
      tabindex="0"
      @click="actionMethod"
      @keyup.enter="actionMethod">
      Custom <span aria-hidden="true">Button</span></div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'CustomButton',
 methods: {
  actionMethod(){
    console.log('I love to be clicked')
  }
 }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.container{
background-color: rgb(246, 220, 220);
padding: 10px;
margin: 20px;
}
    
.primary-button {
outline-offset: 2px;
margin-top: 5px;
display: inline-block;
padding: 10px 20px;
background-color: #007bff; /* Primary color */
color: #ffffff; /* Text color */
border: none;
border-radius: 5px;
font-size: 16px;
cursor: pointer;
text-decoration: none;
transition: background-color 0.3s ease;
}

.primary-button:hover {
background-color: #0056b3; 
}
</style>
