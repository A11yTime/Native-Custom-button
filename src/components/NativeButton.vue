<template>
    <div class="border">
      <h1>Native button</h1>
      <div>
          <button class="button primary" @click="actionButton('Primary')" >Primary <span aria-hidden="true" >Button</span></button>
          <button class="button secondary" @click="actionButton('Secondary')">Secondary <span aria-hidden="true">Button</span></button>
          <button class="button tertiary" @click="actionButton('Tertiary')">Tertiary <span aria-hidden="true">Button</span></button>
      </div>
    </div>
  </template>
  <script>
  export default{
      data(){
          return {
              buttonAction: ''
          }
      },
      methods: {
      actionButton(type){
        const ac = this.buttonAction = type;
        console.log(`${ac } button has been clicked`)
      }
      }
  }
  </script>
  <style scoped>
  .border {
    background-color: rgb(243, 241, 241);
    padding: 10px;
    margin: 20px;
  }
  .button {
    display: inline-block;
    padding: 10px 20px;
    margin: 5px;
    border: none;
    border-radius: 5px;
    cursor: pointer;
    text-align: center;
    text-decoration: none;
    font-size: 16px;
    transition: background-color 0.3s;
  }
  .primary {
    background-color: #007bff;
    color: #fff;
  }
  .secondary {
    background-color: #6c757d;
    color: #fff;
  }
  .tertiary {
    background-color: #f8f9fa;
    color: #212529;
    border: 1px solid #ccc;
  }
  </style>