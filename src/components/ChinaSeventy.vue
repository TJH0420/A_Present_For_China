<template>
  <div class="China">
    <div class="common China_wechat"></div>
    <div class="common China_70"></div>
    <div class="common China_mother"></div>
    <div class="common China_people"></div>
    <div class="common China_web"></div>
  </div>
</template>

<script>
export default {
  name: "ChinaSeventy",
  props: {
    msg: String
  },
  data() {
    return {};
  },
  created() {},
  methods: {}
};
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped>
.common {
  position: absolute;
  width: 5vw;
  height: 5vw;
  box-shadow: 0 0 10px 0 rgba(0, 0, 0, 0.1);
  text-align: center;
  color: red;
  font-size: 4vw;
  -webkit-animation: loop_show 5s linear infinite;
  animation: loop_show 5s linear infinite;
  -webkit-animation-fill-mode: both;
  animation-fill-mode: both;
}
.common::after {
  content: "";
  position: absolute;
  top: 50%;
  left: 0;
  right: 0;
  height: 360px;
  -webkit-transform-origin: top center;
  transform-origin: top center;
  -webkit-animation: inherit;
  animation: inherit;
  -webkit-animation-name: shadow;
  animation-name: shadow;
}
.China_wechat {
  top: calc(100vh - 5vh);
  left: calc(15vw - 5vw);
  background: linear-gradient(45deg, #db6440 0%, #e7802c 100%);
  border-radius: 100%;
}
.China_wechat::after {
  content: "黑叔说前端";
  padding-top: 80%;
  background: linear-gradient(
    -180deg,
    rgba(219, 100, 64, 0.4) 0%,
    rgba(28, 28, 28, 0) 100%
  );
}
.China_70 {
  top: calc(100vh - 5vh);
  left: calc(35vw - 5vw);
  background: linear-gradient(45deg, #c1da39 0%, #dbd813 100%);
  border-radius: 100% 50%;
  -webkit-animation-delay: 0.5s;
  animation-delay: 0.5s;
}
.China_70::after {
  content: "新中国成立七十周年";
  padding-top: 80%;
  background: linear-gradient(
    -180deg,
    rgba(193, 218, 57, 0.4) 0%,
    rgba(28, 28, 28, 0) 100%
  );
}
.China_mother {
  top: calc(100vh - 5vh);
  left: calc(55vw - 5vw);
  background: linear-gradient(45deg, #ea9f45 0%, #f4ee51 100%);
  -webkit-animation-delay: 2s;
  animation-delay: 2s;
}
.China_mother::after {
  content: "祖国万岁";
  padding-top: 80%;
  background: linear-gradient(
    -180deg,
    rgba(234, 159, 69, 0.3) 0%,
    rgba(28, 28, 28, 0) 100%
  );
}
.China_people {
  top: calc(100vh - 5vh);
  left: calc(75vw - 5vw);
  background: linear-gradient(45deg, #22a0f9 0%, #71fdc8 100%);
  -webkit-animation-delay: 1s;
  animation-delay: 1s;
  border-radius: 50% 100%;
}
.China_people::after {
  content: "人民万岁";
  padding-top: 80%;
  background: linear-gradient(
    -180deg,
    rgba(34, 223, 249, 0.4) 0%,
    rgba(28, 28, 28, 0) 100%
  );
}
.China_web {
  top: calc(100vh - 5vh);
  left: calc(95vw - 5vw);
  background: linear-gradient(45deg, #35d37c 0%, #0dce4d 100%);
  -webkit-animation-delay: 2.5s;
  animation-delay: 2.5s;
  border-radius: 100% 100% 0 0;
}
.China_web::after {
  content: "前端万岁";
  padding-top: 80%;
  background: linear-gradient(
    -180deg,
    rgba(53, 211, 124, 0.4) 0%,
    rgba(28, 28, 28, 0) 100%
  );
}
@-webkit-keyframes loop_show {
  0% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  80% {
    -webkit-transform: translateY(-100vh);
    transform: translateY(-100vh);
    opacity: 1;
  }
  100% {
    opacity: 0;
    -webkit-transform: translateY(-100vh);
    transform: translateY(-100vh);
  }
}
@keyframes loop_show {
  0% {
    -webkit-transform: translateY(0);
    transform: translateY(0);
    opacity: 0;
  }
  50% {
    opacity: 1;
  }
  80% {
    -webkit-transform: translateY(-100vh);
    transform: translateY(-100vh);
    opacity: 1;
  }
  100% {
    opacity: 0;
    -webkit-transform: translateY(-100vh);
    transform: translateY(-100vh);
  }
}
@-webkit-keyframes shadow {
  0% {
    -webkit-transform: scaleY(0);
    transform: scaleY(0);
  }
  30% {
    -webkit-transform: scaleY(1);
    transform: scaleY(1);
  }
  100% {
    -webkit-transform: scaleY(0.5);
    transform: scaleY(0.5);
  }
}
@keyframes shadow {
  0% {
    -webkit-transform: scaleY(0);
    transform: scaleY(0);
  }
  30% {
    -webkit-transform: scaleY(1);
    transform: scaleY(1);
  }
  100% {
    -webkit-transform: scaleY(0.5);
    transform: scaleY(0.5);
  }
}
</style>
