<template>
  <div class="hello">
    <img class="head-shot" src="../assets/headshot2.jpg" alt="" />
    <div class="text">
      <h2>Who Am I?</h2>
      <p>{{ whoAmI }}</p>
    </div>
  </div>
</template>

<script>
export default {
  data() {
    return {
      whoAmI: "I’m a full stack software developer with over 20 years of experience as a veterinary nurse. During my time in veterinary care, I provided care for animals while building strong connections with their owners, refining my communication and relationship-building skills. As a life-long problem solver I am always looking for the next challenge to tackle head-on, whether an animal is ill or troubleshooting a computer program. Driven by my pursuit of knowledge, I’m constantly searching for new challenges and any opportunity to expand my skills and competence. My early passion for landscape painting has helped me in develop a keen eye for composition which I now bring to every web design project. In my free time you can find me cooking a delicious dinner, enjoying the great outdoors with my children and pets, or taking in a movie.",
    };
  },
  name: "HelloWorld",
  props: {
    msg: String,
  },
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
h3 {
  margin: 40px 0 0;
}
ul {
  list-style-type: none;
  padding: 0;
}
li {
  display: inline-block;
  margin: 0 10px;
}


.hello .text p {
  color: #023E44;
  
}
</style>
