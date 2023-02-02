<template>

  <div class="container mt-10 justify-center gap-6 flex flex-wrap">
    <div v-for="g in gamers">
      <Fighters :gamer="g" />
    </div>
  </div>

</template>

<script>

// fetch the gamer
const { data: gamers } = await useFetch('https://interactive-production.up.railway.app/gamers')
</script>

<style scoped>

</style>