<template>
  <div>
    <img
      src="https://cdn.jsdelivr.net/gh/zhang13pro/blogImg/img/404.jpg"
      alt=""
    />
    <p class="number">404</p>
    <p class="content">
      Hm,the page you were looking for doesn't seem to exist anymore:(
    </p>
    <button>get back</button>
  </div>
</template>

<script>
export default {};
</script>

<style>
img {
  height: 100vh;
  width: 100vw;
  object-fit: cover;
}

.number {
  color: green;
}

.content {
  color: red;
  font-family: Times New Roman;
  font-size: 22px;
}
</style>