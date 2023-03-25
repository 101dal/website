<template>
    <div>
      <h1>{{ post.title }}</h1>
      <p>{{ post.content }}</p>
    </div>
  </template>
  
  <script>
  export default {
    data() {
      return {
        posts: [
          { id: 1, title: "Mon premier article de blog", content: "Contenu de mon premier article de blog." },
          { id: 2, title: "Mon deuxième article de blog", content: "Contenu de mon deuxième article de blog." },
          { id: 3, title: "Mon troisième article de blog", content: "Contenu de mon troisième article de blog." },
        ],
      };
    },
    computed: {
      post() {
        return this.posts.find((p) => p.id === parseInt(this.$route.params.id));
      },
    },
  };
  </script>
  