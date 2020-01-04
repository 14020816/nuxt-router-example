<template>
  <v-app>
    <div height="56px" app dense> 
      <nuxt-link class="nuxt-link" to='/'>Home page</nuxt-link>
      <nuxt-link class="nuxt-link" to='/page1'>Page 1</nuxt-link>
      <nuxt-link class="nuxt-link" to='/users'>User List</nuxt-link>
    </div>
    <v-content style="margin-left: 10px">
        <nuxt/>
    </v-content>
  </v-app>
</template>

<script>
export default {
  data () {
    return {
      clipped: false,
      drawer: false,
      fixed: false,
      color: "",
      items: [
        {
          icon: 'mdi-apps',
          title: 'Welcome',
          to: '/'
        },
        {
          icon: 'mdi-chart-bubble',
          title: 'Inspire',
          to: '/inspire'
        }
      ],
      miniVariant: false,
      right: true,
      rightDrawer: false,
      title: 'Vuetify.js'
    }
  },
  methods: {
    onClick(){
      // window.alert("Hang click");
      
    }
  }
}
</script>

<style scoped>
  .nuxt-link {
    font-family: 'Times New Roman', Times, serif;
    font-size: 24px;
    color: blue;
    margin-left: 10px;
    margin-right: 10px;
    text-decoration-line: none;
  }
  .nuxt-link:hover{
    color: red;
  }
</style>