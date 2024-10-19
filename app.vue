<template>
  <div>
    <div id="lele-image" :class="{ active: isActive }">
      <img src="/lele.webp" width="200" alt="">
    </div>
    <div id="lele-text" :class="{ active: isActive }">
      <div class="loading-container">
        <div class="smiley">
          <div class="one">H</div>
        </div>
        <div class="smiley">
          <div class="two">A</div>
        </div>
        <div class="smiley">
          <div class="three">P</div>
        </div>
        <div class="smiley">
          <div class="four">P</div>
        </div>
        <div class="smiley">
          <div class="five">Y</div>
        </div>
      </div>
    </div>
    <div :class="{ 'not-loaded': !isLoad }">
      <div class="night"></div>
      <div class="flowers">
        <div class="flower flower--1">
          <div class="flower__leafs flower__leafs--1">
            <div class="flower__leaf flower__leaf--1"></div>
            <div class="flower__leaf flower__leaf--2"></div>
            <div class="flower__leaf flower__leaf--3"></div>
            <div class="flower__leaf flower__leaf--4"></div>
            <div class="flower__white-circle"></div>

            <div class="flower__light flower__light--1"></div>
            <div class="flower__light flower__light--2"></div>
            <div class="flower__light flower__light--3"></div>
            <div class="flower__light flower__light--4"></div>
            <div class="flower__light flower__light--5"></div>
            <div class="flower__light flower__light--6"></div>
            <div class="flower__light flower__light--7"></div>
            <div class="flower__light flower__light--8"></div>

          </div>
          <div class="flower__line">
            <div class="flower__line__leaf flower__line__leaf--1"></div>
            <div class="flower__line__leaf flower__line__leaf--2"></div>
            <div class="flower__line__leaf flower__line__leaf--3"></div>
            <div class="flower__line__leaf flower__line__leaf--4"></div>
            <div class="flower__line__leaf flower__line__leaf--5"></div>
            <div class="flower__line__leaf flower__line__leaf--6"></div>
          </div>
        </div>

        <div class="flower flower--2">
          <div class="flower__leafs flower__leafs--2">
            <div class="flower__leaf flower__leaf--1"></div>
            <div class="flower__leaf flower__leaf--2"></div>
            <div class="flower__leaf flower__leaf--3"></div>
            <div class="flower__leaf flower__leaf--4"></div>
            <div class="flower__white-circle"></div>

            <div class="flower__light flower__light--1"></div>
            <div class="flower__light flower__light--2"></div>
            <div class="flower__light flower__light--3"></div>
            <div class="flower__light flower__light--4"></div>
            <div class="flower__light flower__light--5"></div>
            <div class="flower__light flower__light--6"></div>
            <div class="flower__light flower__light--7"></div>
            <div class="flower__light flower__light--8"></div>

          </div>
          <div class="flower__line">
            <div class="flower__line__leaf flower__line__leaf--1"></div>
            <div class="flower__line__leaf flower__line__leaf--2"></div>
            <div class="flower__line__leaf flower__line__leaf--3"></div>
            <div class="flower__line__leaf flower__line__leaf--4"></div>
          </div>
        </div>

        <div class="flower flower--3">
          <div class="flower__leafs flower__leafs--3">
            <div class="flower__leaf flower__leaf--1"></div>
            <div class="flower__leaf flower__leaf--2"></div>
            <div class="flower__leaf flower__leaf--3"></div>
            <div class="flower__leaf flower__leaf--4"></div>
            <div class="flower__white-circle"></div>

            <div class="flower__light flower__light--1"></div>
            <div class="flower__light flower__light--2"></div>
            <div class="flower__light flower__light--3"></div>
            <div class="flower__light flower__light--4"></div>
            <div class="flower__light flower__light--5"></div>
            <div class="flower__light flower__light--6"></div>
            <div class="flower__light flower__light--7"></div>
            <div class="flower__light flower__light--8"></div>

          </div>
          <div class="flower__line">
            <div class="flower__line__leaf flower__line__leaf--1"></div>
            <div class="flower__line__leaf flower__line__leaf--2"></div>
            <div class="flower__line__leaf flower__line__leaf--3"></div>
            <div class="flower__line__leaf flower__line__leaf--4"></div>
          </div>
        </div>

        <div class="grow-ans" style="--d:1.2s">
          <div class="flower__g-long">
            <div class="flower__g-long__top"></div>
            <div class="flower__g-long__bottom"></div>
          </div>
        </div>

        <div class="growing-grass">
          <div class="flower__grass flower__grass--1">
            <div class="flower__grass--top"></div>
            <div class="flower__grass--bottom"></div>
            <div class="flower__grass__leaf flower__grass__leaf--1"></div>
            <div class="flower__grass__leaf flower__grass__leaf--2"></div>
            <div class="flower__grass__leaf flower__grass__leaf--3"></div>
            <div class="flower__grass__leaf flower__grass__leaf--4"></div>
            <div class="flower__grass__leaf flower__grass__leaf--5"></div>
            <div class="flower__grass__leaf flower__grass__leaf--6"></div>
            <div class="flower__grass__leaf flower__grass__leaf--7"></div>
            <div class="flower__grass__leaf flower__grass__leaf--8"></div>
            <div class="flower__grass__overlay"></div>
          </div>
        </div>

        <div class="growing-grass">
          <div class="flower__grass flower__grass--2">
            <div class="flower__grass--top"></div>
            <div class="flower__grass--bottom"></div>
            <div class="flower__grass__leaf flower__grass__leaf--1"></div>
            <div class="flower__grass__leaf flower__grass__leaf--2"></div>
            <div class="flower__grass__leaf flower__grass__leaf--3"></div>
            <div class="flower__grass__leaf flower__grass__leaf--4"></div>
            <div class="flower__grass__leaf flower__grass__leaf--5"></div>
            <div class="flower__grass__leaf flower__grass__leaf--6"></div>
            <div class="flower__grass__leaf flower__grass__leaf--7"></div>
            <div class="flower__grass__leaf flower__grass__leaf--8"></div>
            <div class="flower__grass__overlay"></div>
          </div>
        </div>

        <div class="grow-ans" style="--d:2.4s">
          <div class="flower__g-right flower__g-right--1">
            <div class="leaf"></div>
          </div>
        </div>

        <div class="grow-ans" style="--d:2.8s">
          <div class="flower__g-right flower__g-right--2">
            <div class="leaf"></div>
          </div>
        </div>

        <div class="grow-ans" style="--d:2.8s">
          <div class="flower__g-front">
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--1">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--2">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--3">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--4">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--5">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--6">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--7">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__leaf-wrapper flower__g-front__leaf-wrapper--8">
              <div class="flower__g-front__leaf"></div>
            </div>
            <div class="flower__g-front__line"></div>
          </div>
        </div>

        <div class="grow-ans" style="--d:3.2s">
          <div class="flower__g-fr">
            <div class="leaf"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--1"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--2"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--3"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--4"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--5"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--6"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--7"></div>
            <div class="flower__g-fr__leaf flower__g-fr__leaf--8"></div>
          </div>
        </div>

        <div class="long-g long-g--0">
          <div class="grow-ans" style="--d:3s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:2.2s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:3.4s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:3.6s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--1">
          <div class="grow-ans" style="--d:3.6s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:3.8s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:4s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:4.2s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--2">
          <div class="grow-ans" style="--d:4s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:4.2s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:4.4s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:4.6s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--3">
          <div class="grow-ans" style="--d:4s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:4.2s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:3s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:3.6s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--4">
          <div class="grow-ans" style="--d:4s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:4.2s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:3s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:3.6s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--5">
          <div class="grow-ans" style="--d:4s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:4.2s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:3s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:3.6s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--6">
          <div class="grow-ans" style="--d:4.2s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:4.4s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:4.6s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:4.8s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>

        <div class="long-g long-g--7">
          <div class="grow-ans" style="--d:3s">
            <div class="leaf leaf--0"></div>
          </div>
          <div class="grow-ans" style="--d:3.2s">
            <div class="leaf leaf--1"></div>
          </div>
          <div class="grow-ans" style="--d:3.5s">
            <div class="leaf leaf--2"></div>
          </div>
          <div class="grow-ans" style="--d:3.6s">
            <div class="leaf leaf--3"></div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>
<script setup>
const isLoad = ref(false);
const isActive = ref(false)
onMounted(() => {
  isLoad.value = true
  isActive.value = true
})


</script>
<style lang="scss">
//ANIMATING Smileys :)
$color-grey: grey;
$color-grey-dark: #333;

.loading-container {
  min-height: 300px;
  overflow: hidden;
  margin: 0 auto;
  position: relative;
  text-align: center;

  &:after {
    content: "Chúc LeLe 20/10 vui vẻ";
    color: #fff;
    font-size: 20px;
    text-align: center;
    display: block;
    letter-spacing: 2px;
    font-weight: bold;
    font-family: "comic sans";
  }


  .smiley {
    position: relative;
    height: 100px;
    width: 40px;
    display: inline-block;
    margin: 0 5px 10px;
    cursor: pointer;

    &:hover>* {
      border-color: $color-grey;
      color: $color-grey;
      animation: jump 0.5s infinite alternate;
      -o-animation: jump 0.5s infinite alternate;
      -ms-animation: jump 0.5s infinite alternate;
      -moz-animation: jump 0.5s infinite alternate;
      -webkit-animation: jump 0.5s infinite alternate;
    }

    &>* {
      position: absolute;
      top: -40px;
      left: 0;
      right: 0;
      height: 40px;
      line-height: 30px;
      text-align: center;
      width: 38px;
      // border: 3px solid $color-grey-dark;
      color: $color-grey-dark;
      padding: 0 0 8px;
      border-radius: 50%;
      margin: 100px auto;
      font-size: 50px;
      font-family: "comic sans ms", sans-serif;
      font-weight: bold;

      transition: color .25s linear, border-color .25s linear;
      // transform: rotate(90deg);
      animation: jump 0.5s infinite alternate;

      -o-transition: color .25s linear, border-color .25s linear;
      -o-transform: rotate(90deg);
      -o-animation: jump 0.5s infinite alternate;

      -moz-transition: color .25s linear, border-color .25s linear;
      // -moz-transform: rotate(90deg);
      -moz-animation: jump 0.5s infinite alternate;

      -webkit-transition: color .25s linear, border-color .25s linear;
      // -webkit-transform: rotate(90deg);
      -webkit-animation: jump 0.5s infinite alternate;
    }

    .one {
      color: #f9ca24;
      animation-delay: 0s;
      -o-animation-delay: 0s;
      -moz-animation-delay: 0s;
      -webkit-animation-delay: 0s;
    }

    .two {
      color: #f0932b;
      animation-delay: 0.1s;
      -o-animation-delay: 0.1s;
      -moz-animation-delay: 0.1s;
      -webkit-animation-delay: 0.1s;
    }

    .three {
      animation-delay: 0.2s;
      -o-animation-delay: 0.2s;
      -moz-animation-delay: 0.2s;
      -webkit-animation-delay: 0.2s;
    }

    .four {
      color: #eb4d4b;
      animation-delay: 0.3s;
      -o-animation-delay: 0.3s;
      -moz-animation-delay: 0.3s;
      -webkit-animation-delay: 0.3s;
    }

    .five {
      color: #6ab04c;
      animation-delay: 0.4s;
      -o-animation-delay: 0.4s;
      -moz-animation-delay: 0.4s;
      -webkit-animation-delay: 0.4s;
    }

  }

  @keyframes jump {
    0% {
      top: -40px;
      -moz-transform: scale(1, 0.7);
    }

    30% {
      -moz-transform: scale(1, 1);
    }

    100% {
      top: -70px;
    }
  }

  @-o-keyframes jump {
    0% {
      top: -40px;
      -moz-transform: scale(1, 0.7);
    }

    30% {
      -moz-transform: scale(1, 1);
    }

    100% {
      top: -70px;
    }
  }

  @-ms-keyframes jump {
    0% {
      top: -40px;
      -moz-transform: scale(1, 0.7);
    }

    30% {
      -moz-transform: scale(1, 1);
    }

    100% {
      top: -70px;
    }
  }

  @-moz-keyframes jump {
    0% {
      top: -40px;
      -moz-transform: scale(1, 0.7);
    }

    30% {
      -moz-transform: scale(1, 1);
    }

    100% {
      top: -70px;
    }
  }

  @-webkit-keyframes jump {
    0% {
      top: -40px;
      -webkit-transform: scale(1, 0.7);
    }

    30% {
      -webkit-transform: scale(1, 1);
    }

    100% {
      top: -70px;
    }
  }
}
</style>
<style>
#lele-text {
  position: fixed;
  top: 25%;
  right: 0%;
  z-index: 1000;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

#lele-image {
  position: fixed;
  top: 0%;
  right: 0%;
  z-index: 999;
  width: 100%;
  display: flex;
  align-items: center;
  justify-content: center;
}

#lele-image,
#lele-text {
  opacity: 0;
}

/* Khi có class active thì bắt đầu animation */
#lele-image.active {
  animation: slideDown 2s ease forwards;
}

#lele-text.active {
  animation: slideInLeft 1.5s ease forwards;
}

/* Keyframes cho #lele-image (từ trên xuống) */
@keyframes slideDown {
  0% {
    transform: translateY(-100%);
    opacity: 0;
  }

  100% {
    transform: translateY(0);
    opacity: 1;
  }
}

/* Keyframes cho #lele-text (từ trái qua) */
@keyframes slideInLeft {
  0% {
    transform: translateX(-100%);
    opacity: 0;
  }

  100% {
    transform: translateX(0);
    opacity: 1;
  }
}
</style>