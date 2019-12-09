<template>
  <div class="home">
    <b-container class="mt-4 mb-4">
      <h1>Girls Who Code at Harrisonburg High School</h1>
      <p>Welcome to the Harrisonburg High School Girls Who Code project gallery! You can find projects by our club members below. Feel free to explore and share!</p>
    </b-container>
    <hr>
    <b-container>
      <Project v-for="post in posts" v-bind:key="post.id" v-bind="post" />
    </b-container>

  </div>
</template>
<script>
import Project from "@/components/Project.vue";

export default {
  components: {
    Project
  },
  data() {
    return {
      posts: [
        { 
          id: "0",
          title: "Click the Balloons!",
          author: "Slaw Paw",
          description: "This project was made with Scratch, a block-based coding language created by the MIT Media Lab.",
          link: "https://scratch.mit.edu/projects/351891137/fullscreen/",
          img: "https://picsum.photos/600/300/?image=25"
        }
      ]
    }
  }
}

</script>
