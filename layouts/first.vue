<script>
export default {
  props: ['slideTitle'],
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
  <div class="slidev-layout">
    <div class="my-auto">
    <h1 class="slideTitle">{{slideTitle}}</h1>
      <slot />
    <p>
    {{date}}
    </p>
    </div>
  </div>
</template>

<style>
.my-auto{
text-align:center;
padding:1rem;
}
.slideTitle{
color: #003577 !important;
font-size: 4rem !important;
line-height: 4rem !important;
}
.slidev-layout h2,h3 {
  line-height: 3rem !important;
}
</style>

