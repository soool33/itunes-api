<template>
<div>
    <h1> recherche iTunes</h1>
    <br />
    <form @submit.prevent="submit">
        <input placeholder="album name" v-model="search" autofocus />
    </form>
</div>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  components: {

  },
  data() {
     return {
         search: ''
     }
  },
  methods: {
      submit(event) {
          this.$router.push(`results/${this.search}`);
      }
  }

}
</script>

<style>
    * {
        text-align: center;
    }

    h1 {
        padding: 20px;
    }
</style>
