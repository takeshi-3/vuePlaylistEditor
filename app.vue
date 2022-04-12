<script lang="ts">
import { defineComponent } from 'vue';
import Header from './components/Header.vue';
import Login from './components/Login.vue';
import Playlist from './components/Playlist.vue';

export default defineComponent({
  components: {
    Header,
    Login,
    Playlist,
  },
  setup() {
    
  },
})
</script>

<template>
  <div>
    <Header />
    <Login />
    <div>
      <Playlist />
      <!-- <SerchEngine /> -->
    </div>
  </div>
</template>

<style>
* {
  background-color: #EBECF0;
}
body {
  padding: 24px;
}
</style>