<template>
  <div class="app">
    <the-header></the-header>
    <badge-list></badge-list>
    <user-info
      :full-name="activeUser.name"
      :info-text="activeUser.description"
      :role="activeUser.role"
    >
    </user-info>
  </div>
</template>

<script>
import TheHeader from './components/TheHeader.vue';
import BadgeList from './components/BadgeList.vue';
import UserInfo from './components/UserInfo.vue';


export default {
  components: {
    TheHeader,
    BadgeList,
    UserInfo,
  },

  data() {
    return {
      activeUser: {
        name: 'Hasmik Mejlumyan',
        description: 'Site owner and admin',
        role: 'admin',
      },
    };
  },
};
</script>

<style>
  body {
    margin: 0;
  }

  .app {
    width: 100%;
    display: flex;
    justify-content: center;
    align-items: center;
    flex-direction: column;
  }
</style>