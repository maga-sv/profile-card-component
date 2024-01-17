<script setup>
import BgPatternBottom from "./assets/images/BgPatternBottom.vue";
import BgPatternTop from "./assets/images/BgPatternTop.vue";
import Card from "./components/Card/Card.vue";

</script>

<template>
  <main>
    <BgPatternTop class="pattern__top" />
    <BgPatternBottom class="pattern__bottom" />

    <section class="user">

      <div class="container">

        <Card />

      </div>

    </section>
  </main>
</template>

<style lang="scss" scoped>
main {
  position: relative;
  height: 100vh;
  overflow: hidden;
  display: grid;
  place-items: center;

  .pattern {
    &__top,
    &__bottom {
      position: absolute;
      z-index: -1;
    }

    &__top {
      transform: translate(-50%, -50%);
    }
    
    &__bottom {
      transform: translate(50%, 50%);
    }
  }
}
</style>
