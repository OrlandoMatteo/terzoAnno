<script>
export default {
  computed: {
    date() {
      const today = new Date();
      const yyyy = today.getFullYear();
      let mm = today.getMonth() + 1; // Months start at 0!
      let dd = today.getDate();
      const formattedToday = dd + "/" + mm + "/" + yyyy;
      return formattedToday;
    },
  },
};
</script>
<template>
    <img src="/assets/scudo.jpeg" style="position:fixed;top:0.8rem;right:0.8rem;width:12rem;z-index:-1">
  <footer
    class="
      absolute
      p-4
      mt-auto
      flex
      justify-between
      items-center
      w-full
      text-white
      z-10
    "
    style="font-size:0.75rem;bottom:-1.2rem"
    v-if="$slidev.nav.currentPage!=1"
  >
    <i>PhDMAN</i>
    <i>{{ date }}</i>
    <i>Matteo Orlando</i>
    <i>{{$slidev.nav.currentPage-1}}</i>
  </footer>
</template>
