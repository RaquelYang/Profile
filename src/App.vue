<template>
  <v-app class="app">
    <v-main>
      <router-view/>
    </v-main>
  </v-app>
</template>
<style lang="scss">
.v-main__wrap{
  background-color: #eeeeee22;
}
</style>
<script>

export default {
  name: 'App',
  data: () => ({
  })
}
</script>
