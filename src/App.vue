<template>
  <div id="app">
    <header>
      <h1>Matthew Brown</h1>

      <p>Software developer | Veterinary Nurse | Artist | Movie Connoisseur </p>
    <nav>
      <router-link :to="{name: 'home'}">Home</router-link> |
      <router-link :to="{name: 'portfolio'}">Portfolio</router-link> |
      <router-link :to="{name: 'resume'}">Resume</router-link>
    </nav>
    </header>
    <router-view/>
  </div>
</template>

<script>
export default {
  title: 'Matthew Brown'
}
</script>

<style>
*{
  margin: 0px;
  padding: 0px;
  
}
#app {
  font-family: Poppins, Avenir, Helvetica, Arial, sans-serif;
  -webkit-font-smoothing: antialiased;
  -moz-osx-font-smoothing: grayscale;
  text-align: center;
  color: #2c3e50;
  background-color: #FFDDD2;
  min-height: 100%;
}

header {
  display: flex;
  flex-direction:column;
  justify-content: space-between;
  padding: 0px, 20px;
  /* background-image: linear-gradient(-160deg, rgba(0, 109, 119, 1) 15%, rgba(0, 84, 94, 1) 35%, rgba(0, 61, 71, 1) 50%, rgba(0, 39, 48, 1) 65%, rgba(0, 13, 28, 1) 85%, rgba(0, 0, 0, 1) 100%);  */
  background-image: radial-gradient(circle farthest-corner at center, rgba(0, 109, 119, 1) 15%, rgba(0, 84, 94, 1) 35%, rgba(0, 61, 71, 1) 50%, rgba(0, 39, 48, 1) 65%, rgba(0, 13, 28, 1) 85%, rgba(0, 0, 0, 1) 100%);
  height: 300px;
  
}

body {
  min-height: 100%;
  background-color: #FFDDD2;
}

h1 {
  color:#EDF6F9;
  font-size: 150px;
  
  
}

h2 {
  color: #006D77;
  font-size: 40px;
}


nav {
  padding: 30px;
  background-color:#E29578 ;
}

nav a {
  font-weight: bold;
  color: #EDF6F9;
  text-decoration: none;
  font-size: 20px;
}

nav a.router-link-exact-active {
  color: #006D77;
}

.head-shot {
  width: 400px;
  margin: 200px;
  
}

.hello {
  display: grid;
  grid-template-columns: auto 1fr;
  column-gap: 20px;
  align-items: center;
}

p {
  color: #023E44;
  padding: 0px 0px 30px;
 
}

header p {
  font-size: 20px;
  color: #EDF6F9
}

.hello .text p {
  font-size: 30px;
  color: #023E44;
  padding: 20px 10px;
  margin-right: 40px;
  
}

.text h2{
  font-size: 60px;
  padding: 20px;
  color: #023E44;
}
</style>
