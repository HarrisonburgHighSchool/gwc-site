<template>
  <div class="home">
    <b-container class="mt-4 mb-4">
      <h1>Girls Who Code at Harrisonburg High School</h1>
      <p>Welcome to the Harrisonburg High School Girls Who Code project gallery! You can find projects by our club members below. Feel free to explore and share!</p>
    </b-container>

    <hr>
    <b-container>
      <b-card-group deck>
        <Project v-for="post in posts" v-bind:key="post.id" v-bind="post" />
      </b-card-group>
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
          title: "Paddle & Ball",
          author: "Slaw",
          description: "This project was made with Scratch, a block-based coding language created by the MIT Media Lab.",
          link: "https://scratch.mit.edu/projects/351891137/fullscreen/",
          img: "https://raw.githubusercontent.com/HarrisonburgHighSchool/gwc-site/master/src/assets/slaw-paw-game.png"
        },
        { 
          id: "1",
          title: "Click the Balloons!",
          author: "Ka The",
          description: "This project was made with Scratch, a block-based coding language created by the MIT Media Lab.",
          link: "https://scratch.mit.edu/projects/351900021/fullscreen",
          img: "https://raw.githubusercontent.com/HarrisonburgHighSchool/gwc-site/master/src/assets/ka-the-game.png"
        },
        { 
          id: "2",
          title: "How To Learn Cursive",
          author: "Arianna",
          description: "This project was made with HTML and CSS, the language of web development.",
          link: "#",
          img: "https://via.placeholder.com/350x250"
        },
        { 
          id: "3",
          title: "Rakuten Viki Dramafever and Hulu",
          author: "Chekna",
          description: "This project was made with HTML and CSS, the language of web development.",
          link: "https://trinket.io/html/95f1fbc609?e=1",
          img: "https://raw.githubusercontent.com/HarrisonburgHighSchool/gwc-site/master/src/assets/chekna.png"
        },
        { 
          id: "4",
          title: "Be Happy!",
          author: "Asende",
          description: "This project was made with HTML and CSS, the language of web development.",
          link: "https://trinket.io/html/e06afa9bb4?e=1",
          img: "https://raw.githubusercontent.com/HarrisonburgHighSchool/gwc-site/master/src/assets/asende.png"
        },
        { 
          id: "5",
          title: "Pronounce Correctly",
          author: "Melve",
          description: "This project was made with Thunkable, a block-based coding language for creating mobile applications for iPhone and Android.",
          link: "#",
          img: "https://via.placeholder.com/350x250"
        },
        { 
          id: "5",
          title: "Placeholder",
          author: "Rita",
          description: "This project was made with HTML and CSS, the language of web development.",
          link: "#",
          img: "https://via.placeholder.com/350x250"
        }
      ]
    }
  }
}

</script>
