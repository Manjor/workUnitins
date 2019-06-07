<template>
  <v-app>
    <v-container>
      <v-layout>
        <v-flex xs8 offset-md-2>
            <Content title="Primeiro"/>
        </v-flex>
      </v-layout>
    </v-container>
  </v-app>
</template>

<script>
import Content from '@/components/template/Content'
export default {
  name: 'App',
  components: {
    Content
  },
  data () {
    return {
      //
    }
  }
}
</script>
<style>
  #container{
    margin-top: 5%;
  }
</style>

