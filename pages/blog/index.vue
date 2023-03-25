<template>
    <div>
      <h1>Blog</h1>
      <ul>
        <li v-for="post in posts" :key="post.id">
          <nuxt-link :to="`/blog/${post.id}`">{{ post.title }}</nuxt-link>
        </li>
      </ul>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        posts: [
          { id: 1, title: "Mon premier article de blog" },
          { id: 2, title: "Mon deuxième article de blog" },
          { id: 3, title: "Mon troisième article de blog" },
        ],
      };
    },
  };
  </script>
  