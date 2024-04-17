<template>
  <div>
    <a :href="html - url">
      <img class="repo-image" :src="imageSrc" alt="" />
    </a>
    <p><a :href="html_url">{{ title }}</a></p>
    <p>{{ id }}</p>
  </div>
</template>

<script>
export default {
    name:'HelloWorld',
    props: {
        title: String,
        html_url: String,
        imageSrc: String,
        id: Number,
    }
};
</script>

<style scoped>
h3 {
  margin: 40px;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}
.repo-image {
  width: 400px;
}
</style>