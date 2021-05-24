<template>
  <div>
    <img
      src="https://cdn.jsdelivr.net/gh/zhang13pro/blogImg/img/404.jpg"
      alt=""
    />
    <div class="text">
      <p class="number">404</p>
      <p class="content">
        Hm,the page you were looking for doesn't seem to exist anymore :(
      </p>
      <button class="back" @click="reback">Back Home</button>
    </div>
  </div>
</template>

<script>
export default {
  methods: {
    reback() {
      alert("go home");
    },
  },
};
</script>

<style lang="stylus">
@import "../styles/responsive.styl"

#app
  margin 0

img
  height: 100vh;
  width: 100vw;
  object-fit: cover;

.text
  position fixed
  top 50%
  left 50%
  transform translateX(-50%)
  // transform translateY(-50%)
  perspective 31.25rem
  // perspective-origin 50% 50%

.number
  margin 0 auto
  color lightpink
  font-size 2rem
  text-shadow 5px 1px 5px gold
  transform translate3d(3px,-3px,-200px) rotateX(-9deg) rotateY(-22deg)

.content
  margin .625rem 0 0
  color lightpink
  font-family Times New Roman
  transform translate3d(3px,-3px,-100px) rotateX(-9deg) rotateY(-22deg)

.back
  margin 1.875rem 0 0
  height 1.875rem
  width 6.25rem
  font-weight bold
  transform translate3d(3px,-3px,-100px) rotateX(-9deg) rotateY(-22deg)
  border-radius .3125rem
</style>
