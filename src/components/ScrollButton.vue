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
        <span><i class="fa-solid fa-angles-up fs-2"></i></span>
  </div>
</template>

<style lang="scss" scoped>
.scroll-btn {
//   display: none;
  position: fixed;
  bottom: 100px;
  right: 20px;
  background-color: #F9AA01;
  color: black;
  padding: 20px;
  border-radius: 0%;
  transform:  rotate(45deg);
  cursor: pointer;
  z-index: 1000;
    span{
        display: inline-block;
        transform: rotate(-45deg);
     }
}

.scroll-btn.show {
  display: block;
}
</style>
