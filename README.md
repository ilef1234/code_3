<template>
    <div>
      <h1>{{ firstname }}</h1> 
      <h1>{{ lastname}}</h1> 
      <h1>{{ address }}</h1> 
      <p>{{ mydetails }}</p>
    </div>
  </template>
  
  <script setup>
  import { ref } from 'vue';
  
  const firstname = ref('Ria');
  const lastname = ref('Singh');
  const address = ref('Mumbai');
  const mydetails=ref(`I am ${firstname.value} ${lastname.value}`);
  
  
  
  </script>
  
  
  <style>
  #app {
    text-align: center;
    margin-top: 2rem;
  }
  
  p {
    font-size: 1.5rem;
  }
  
  @media (min-width: 1024px) {
    #app {
      margin-top: 4rem;
    }
  }
  </style>
  
