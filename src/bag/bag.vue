<template>
  <div class="container">
    <div class="ul">
      <div class="li">热烈欢迎小刘同学加入了我们！</div>
      <div class="li">热烈欢迎小邓同学加入了我们！</div>
      <div class="li">热烈欢迎小李同学加入了我们！</div>
      <div class="li">热烈欢迎小王同学加入了我们！</div>
          <!--   插入用于填充的数据数据 --> 
      <div class="li">热烈欢迎小刘同学加入了我们！</div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'dz-bag',
  props: ['value'],
  data() {
    return {
      text: ''
    }
  },
  mounted() {
    console.log(this.value)
  }
}
</script>

<style scoped>
.container {
  width: 100%;
  height: 50px;
  background-color: #0e88eb;
  border-radius: 25px;
  position: relative;
  /* overflow: hidden; */
}
.container .ul {
  width: 100%;
  height: 250px;
  left: 0;
  top: 0;
  /* animation-name: scroll;
  animation-duration: 5s;
  animation-timing-function: linear;
  animation-iteration-count: infinite; */
  /* 动画属性简写 */
  animation: scroll 5s linear infinite forwards;
}
.container .ul .li {
  height: 50px;
  line-height: 50px;
  color: #fff;
  text-align: center;
}
@keyframes scroll {
  0% {
    transform: translate(0, 0);
  }
  100% {
    transform: translate(0, -200px);
  }
}
</style>