<script>
export default {
  data() {
    return {
      showScrollButton: false
    };
  },
  methods: {
    checkScroll() {
      this.showScrollButton =
        document.body.scrollTop > 20 || document.documentElement.scrollTop > 20;
    },
    scrollToTop() {
      window.scrollTo({
        top: 0,
        behavior: "smooth"
      });
    }
  },
  mounted() {
    window.addEventListener("scroll", this.checkScroll);
  },
  beforeUnmount() {
    window.removeEventListener("scroll", this.checkScroll);
  }
};
</script>

<template>
    <div v-if="showScrollButton" class="scroll-btn" @click="scrollToTop">
        <i class="fa-solid fa-angles-up fs-2"></i>
  </div>
</template>

<style lang="scss" scoped>
.scroll-btn {
//   display: none;
  position: fixed;
  bottom: 20px;
  right: 20px;
  background-color: #F9AA01;
  color: white;
  padding: 20px;
  border-radius: 50%;
  cursor: pointer;
  z-index: 1000;
}

.scroll-btn.show {
  display: block;
}
</style>
