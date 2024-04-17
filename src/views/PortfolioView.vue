<template>
  <div>
    <div class="repos">
        <div class="columns" v-for="project in data" :key="project.id">
            <repo-component 
            :title='project.name'
            :html_url='project.html_url'
            :imageSrc='require(`../assets/images/github-images/${project.name}.png`)' 
            :id="project.id"/>
        </div>
    </div>
  </div>
</template>

<script>
import githubService from "../services/GitHubService";
import RepoComponent from "@/components/RepoComponent.vue";

export default {
  data() {
    return {
      data: null,
    };
  },
  components : {
     RepoComponent
  },
  mounted() {
    githubService.getRepos().then((response) => {
      this.data = response.data.filter((project) => {
        return (
          project.name === "meterToFeetConv" ||
          project.name === "KitchenConvertor" ||
          project.name === "MovieDataBase"
        );
      });
    });
  },
};
</script>

<style scoped>

.repos {
    display: flex;
    justify-content: space-around;
    margin: 20px;
    padding: 100px;
    color: #006D77;
    
}

.column {
  margin: 20px;
}
</style>