<template>
  <v-layout
    row
    justify-center
    align-center
  >
    <v-flex :key="items" v-for="items in 8">
      <v-img src="https://camo.githubusercontent.com/06b2f979b4fbab8f1822cab69783700f0afa1f90/68747470733a2f2f6e7578746a732e6f72672f6d6574615f3430302e706e67"></v-img>
    </v-flex>
  </v-layout>
</template>

<script>
import Logo from '~/components/Logo.vue'
import VuetifyLogo from '~/components/VuetifyLogo.vue'

export default {
  // layout: 'login',
  name: 'page1',
  layout: 'default',
  components: {
    Logo,
    VuetifyLogo
  }
}
</script>
