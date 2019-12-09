<template>
  <div class="project">
    <b-card
      :title="title"
      :sub-title="'by ' + author"
      :img-src="img"
      :img-alt="img"
      img-top
      tag="project"
      style="max-width: 20rem;"
      class="mb-2"
    >
      <b-card-text>
        {{description}}
      </b-card-text>

      <b-button :href="link" variant="primary">Visit project</b-button>
    </b-card>
  </div>
</template>

<script>
  export default {
    props: {
      id: String,
      title: String,
      author: String,
      description: String,
      link: String,
      img: String
    },
  }
</script>