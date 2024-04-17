<template>
  <div class="resume">
    <VuePdfEmbed :source="resume" style="height: 100vh; width: 100vw;"  />
  </div>
</template>

<script>
import VuePdfEmbed from 'pdf-viewer-vue/dist/vue2-pdf-viewer'

export default {
    data(){
        return{
            resume: 'MB-Resume.pdf'
        }
    },
    components: {
        VuePdfEmbed,
    }

}
</script>

<style>
.resume {
  margin-top: 3%;
}
</style>