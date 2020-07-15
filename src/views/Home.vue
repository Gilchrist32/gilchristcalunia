<template>
  <div class="home">
    <Infohome />
  </div>
</template>

<script>
// @ is an alias to /src

export default {
  name: 'Home',
  components: {
    Infohome: () => import('@/components/Infohome.vue')
  }
}
</script>
