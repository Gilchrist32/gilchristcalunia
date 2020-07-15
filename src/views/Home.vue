<template>
  <div class="home">
    <Infohome />
  </div>
</template>

<script>
export default {
  name: "Home",
  components: {
    Infohome: () => import('@/components/Infohome.vue')
  }
}
</script>