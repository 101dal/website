<template>
    <nav>
      <ul>
        <li><nuxt-link to="/">Accueil</nuxt-link></li>
        <li><nuxt-link to="/blog">Blog</nuxt-link></li>
        <li><nuxt-link to="/about">À propos</nuxt-link></li>
      </ul>
    </nav>
  </template>
  
  <style>
  nav {
    background-color: #333;
    color: white;
  }
  
  ul {
    list-style: none;
    margin: 0;
    padding: 0;
  }
  
  li {
    display: inline-block;
    margin-right: 1em;
  }
  
  a {
    color: white;
    text-decoration: none;
  }
  </style>
  