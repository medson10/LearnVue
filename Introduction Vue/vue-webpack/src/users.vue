<template>
  <div>
    <h1>Users overview</h1>
    <p>TeamID is {{ $route.params.teamId }}</p>
    <button type="button" name="button" @click="goHome">Go home</button>
  </div>
</template>

<script type="text/javascript">
  export default {
    watch: {
      '$route' (to, from) {
        // alert(to.params.teamId);
      }
    },
    created() {
      // alert(this.$route.params.teamId);
    },
    methods: {
      goHome() {
        this.$router.push('/');
      }
    }
  }
</script>
