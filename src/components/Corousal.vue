<template>
  <div id="slider">
    <div class="slides">
      <div class="slider">
        <div class="legend"></div>
        <div class="content">
          <div class="content-txt">
            <h3>Workshop</h3>
            <h1>Merapi Lava Tour</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, vel.</p>
            <rate />
          </div>
        </div>
        <div class="image">
          <img src="https://files.selenago.com/sandbox/fc88e09f-5eed-4b35-8ddc-8f87695dafa7.jpg" />
        </div>
      </div>
      <div class="slider">
        <div class="legend"></div>
        <div class="content">
          <div class="content-txt">
            <h1>Merapi Lava Tour</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, vel.</p>
            <rate />
          </div>
        </div>
        <div class="image">
          <img src="https://files.selenago.com/sandbox/462ba615-db81-49f9-adff-796f325b0db0.JPG" />
        </div>
      </div>
      <div class="slider">
        <div class="legend"></div>
        <div class="content">
          <div class="content-txt">
            <h1>Merapi Lava Tour</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, vel.</p>
            <rate />
          </div>
        </div>
        <div class="image">
          <img src="https://files.selenago.com/sandbox/770df2c6-fe51-4a84-a403-ebe66bf7bf2d.JPG" />
        </div>
      </div>
      <div class="slider">
        <div class="legend"></div>
        <div class="content">
          <div class="content-txt">
            <h1>Merapi Lava Tour</h1>
            <p>Lorem ipsum dolor sit amet consectetur adipisicing elit. Praesentium, vel.</p>
            <rate />
          </div>
        </div>
        <div class="image">
          <img src="https://files.selenago.com/sandbox/5b22f599-877a-4069-8de8-215033c1068c.jpg" />
        </div>
      </div>
    </div>
    <div class="switch">
      <ul>
        <li>
          <div class="on"></div>
        </li>
        <li></li>
        <li></li>
        <li></li>
      </ul>
    </div>
  </div>
</template>
<script>
import rate from "./Rate.vue";
export default {
  components: {
    rate
  }
};
</script>

<style scoped>
/* Reset */
* {
  margin: 0;
  padding: 0;
}
h1 {
  color: white;
}
h2 {
  padding-bottom: 20px;
}
h3 {
  color: #fff;
}
body {
  min-width: 900px;
}
/* Slider */
#slider {
  width: 100%;
  height: 500px;
  position: relative;
  overflow: hidden;
}
@keyframes load {
  from {
    left: -100%;
  }
  to {
    left: 0;
  }
}
.slides {
  width: 400%;
  height: 100%;
  position: relative;
  -webkit-animation: slide 30s infinite;
  -moz-animation: slide 30s infinite;
  animation: slide 30s infinite;
}
.slider {
  width: 25%;
  height: 100%;
  float: left;
  position: relative;
  z-index: 1;
  overflow: hidden;
}
.slide img {
  width: 100%;
  height: 100%;
}
.slide img {
  width: 100%;
  height: 100%;
}
.image {
  width: 100%;
  height: 100%;
}
.image img {
  width: 100%;
  height: 100%;
}

/* Legend */
.legend {
  border: 310px solid transparent;
  border-left: 800px solid rgba(52, 73, 94, 0.7);
  border-bottom: 0;
  position: absolute;
  bottom: 0;
}

/* Contents */
.content {
  width: 100%;
  height: 100%;
  position: absolute;
  overflow: hidden;
}
.content-txt {
  width: 400px;
  height: 150px;
  float: left;
  position: relative;
  top: 300px;
  -webkit-animation: content-s 7.5s infinite;
  -moz-animation: content-s 7.5s infinite;
  animation: content-s 7.5s infinite;
  color: white;
  margin-left: 15px;
  padding-bottom: 15px;
}
.content-txt h2 {
  font-family: Arial;
  text-transform: uppercase;
  font-size: 14px;
  color: #fff;
  text-align: left;
}
.content-txt p {
  font-family: arial;
  font-weight: normal;
  font-size: 14px;
  font-style: italic;
  color: #fff;
  text-align: left;
}

/* Switch */
.switch {
  width: 120px;
  height: 10px;
  position: absolute;
  bottom: 10px;
  z-index: 99;
  left: 30px;
}
.switch > ul {
  list-style: none;
}
.switch > ul > li {
  width: 10px;
  height: 10px;
  border-radius: 50%;
  background: #333;
  float: left;
  margin-right: 5px;
  cursor: pointer;
}
.switch ul {
  overflow: hidden;
}
.on {
  width: 100%;
  height: 100%;
  border-radius: 50%;
  background: #f39c12;
  position: relative;
  -webkit-animation: on 30s infinite;
  -moz-animation: on 30s infinite;
  animation: on 30s infinite;
}

/* Animation */
@-webkit-keyframes slide {
  0%,
  100% {
    margin-left: 0%;
  }
  21% {
    margin-left: 0%;
  }
  25% {
    margin-left: -100%;
  }
  46% {
    margin-left: -100%;
  }
  50% {
    margin-left: -200%;
  }
  71% {
    margin-left: -200%;
  }
  75% {
    margin-left: -300%;
  }
  96% {
    margin-left: -300%;
  }
}
@-moz-keyframes slide {
  0%,
  100% {
    margin-left: 0%;
  }
  21% {
    margin-left: 0%;
  }
  25% {
    margin-left: -100%;
  }
  46% {
    margin-left: -100%;
  }
  50% {
    margin-left: -200%;
  }
  71% {
    margin-left: -200%;
  }
  75% {
    margin-left: -300%;
  }
  96% {
    margin-left: -300%;
  }
}
@keyframes slide {
  0%,
  100% {
    margin-left: 0%;
  }
  21% {
    margin-left: 0%;
  }
  25% {
    margin-left: -100%;
  }
  46% {
    margin-left: -100%;
  }
  50% {
    margin-left: -200%;
  }
  71% {
    margin-left: -200%;
  }
  75% {
    margin-left: -300%;
  }
  96% {
    margin-left: -300%;
  }
}

@-webkit-keyframes content-s {
  0% {
    left: -420px;
  }
  10% {
    left: 0px;
  }
  30% {
    left: 0px;
  }
  40% {
    left: 0px;
  }
  50% {
    left: 0px;
  }
  60% {
    left: 0px;
  }
  70% {
    left: 0;
  }
  80% {
    left: -420px;
  }
  90% {
    left: -420px;
  }
  100% {
    left: -420px;
  }
}
@-moz-keyframes content-s {
  0% {
    left: -420px;
  }
  10% {
    left: 0px;
  }
  30% {
    left: 0px;
  }
  40% {
    left: 0px;
  }
  50% {
    left: 0px;
  }
  60% {
    left: 0px;
  }
  70% {
    left: 0;
  }
  80% {
    left: -420px;
  }
  90% {
    left: -420px;
  }
  100% {
    left: -420px;
  }
}
@keyframes content-s {
  0% {
    left: -420px;
  }
  10% {
    left: 20px;
  }
  15% {
    left: 0px;
  }
  30% {
    left: 0px;
  }
  40% {
    left: 0px;
  }
  50% {
    left: 0px;
  }
  60% {
    left: 0px;
  }
  70% {
    left: 0;
  }
  80% {
    left: -420px;
  }
  90% {
    left: -420px;
  }
  100% {
    left: -420px;
  }
}

@-webkit-keyframes on {
  0%,
  100% {
    margin-left: 0%;
  }
  21% {
    margin-left: 0%;
  }
  25% {
    margin-left: 15px;
  }
  46% {
    margin-left: 15px;
  }
  50% {
    margin-left: 30px;
  }
  71% {
    margin-left: 30px;
  }
  75% {
    margin-left: 45px;
  }
  96% {
    margin-left: 45px;
  }
}

@-moz-keyframes on {
  0%,
  100% {
    margin-left: 0%;
  }
  21% {
    margin-left: 0%;
  }
  25% {
    margin-left: 15px;
  }
  46% {
    margin-left: 15px;
  }
  50% {
    margin-left: 30px;
  }
  71% {
    margin-left: 30px;
  }
  75% {
    margin-left: 45px;
  }
  96% {
    margin-left: 45px;
  }
}

@keyframes on {
  0%,
  100% {
    margin-left: 0%;
  }
  21% {
    margin-left: 0%;
  }
  25% {
    margin-left: 15px;
  }
  46% {
    margin-left: 15px;
  }
  50% {
    margin-left: 30px;
  }
  71% {
    margin-left: 30px;
  }
  75% {
    margin-left: 45px;
  }
  96% {
    margin-left: 45px;
  }
}

/* main */
/* Reset */
a {
  text-decoration: none;
  color: inherit;
}
</style>