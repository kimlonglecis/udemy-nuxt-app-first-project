<template>
  <div>
    <TheHeader @sidenavToggle="displaysidenav = !displaysidenav"/>
    <TheSidenav
      :show="displaysidenav"
      @close="displaysidenav = false"
    />
    <nuxt />
  </div>
</template>

<script>
import TheHeader from "@/components/Navigation/TheHeader"
import TheSidenav from "@/components/Navigation/TheSidenav"

export default {
  components: {
    TheHeader,
    TheSidenav
  },
  data() {
    return {
      displaysidenav: false
    }
  }
}
</script>

<style lang="sass">
  body
</style>
