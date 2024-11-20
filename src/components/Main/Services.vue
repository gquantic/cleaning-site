<script lang="ts" setup>
import { onMounted, ref } from 'vue'

const services = ref({})

services.value = [
  {
    title: 'Уборка жилых помещений',
    price: 400,
  },
  {
    title: 'Уборка коммерческих помещений',
  },
  {
    title: 'Уборка санитарных помещений',
  },
  {
    title: 'Уборка ковров и мягкой мебели',
  },
  {
    title: 'Экологическая уборка',
  },
  {
    title: 'Дополнительные <br> услуги',
    disable_img: true,
    full_width: true,
  },
]
</script>

<template>
  <div class="calc-block">
    <div class="container">
      <h2 class="title">Услуги</h2>

      <div class="services-block">
        <div
          :class="'services-block__item w-full-' + (item?.full_width ?? false)"
          v-for="item in services"
        >
          <p class="go">подробнее</p>

          <div class="item__inner">
            <b v-html="item?.title"></b>

            <svg
              width="37"
              height="37"
              viewBox="0 0 27 27"
              fill="none"
              xmlns="http://www.w3.org/2000/svg"
            >
              <circle cx="13.5" cy="13.5" r="13.5" fill="#DF6C2D" />
              <path
                d="M11 17L18 10"
                stroke="white"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
              <path
                d="M11 10H18V17"
                stroke="white"
                stroke-linecap="round"
                stroke-linejoin="round"
              />
            </svg>
          </div>
          <div class="img-block">
            <img
              src="/src/assets/clean_bg.png"
              v-if="(item?.disable_img ?? false) === false"
              alt=""
            />
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.calc-block {
  background: #fff;
}

.services-block {
  display: flex;
  justify-content: start;
  flex-wrap: wrap;

  &__item {
    width: 225px;
    height: 273px;
    margin-right: 34px;
    padding: 16px;
    background: #f8f8f8;
    margin-bottom: 34px;
    transition: 0.2s;

    &:hover {
      background: #df6c2d;
      cursor: pointer;
      color: #fff;

      .go {
        background: #fff;
        color: #df6c2d;
      }

      svg {
        circle {
          fill: #fff;
        }

        path {
          stroke: #df6c2d;
        }
      }
    }

    svg {
      position: absolute;
      top: 0;
      right: 0;
      margin-right: 20px;
      margin-top: 50px;
    }

    .img-block {
      width: 100%;
      text-align: center;
      margin-top: 20px;
    }

    &.w-full-true {
      width: 484px;

      .img-block {
        text-align: right;
      }
    }

    .go {
      background: #df6c2d;
      width: fit-content;
      margin-bottom: 0;
      color: #fff;
      padding: 2px 13px;
    }

    .item__inner {
      padding: 13px 5px;
      position: relative;

      b {
        font-size: 17px;
        line-height: 17px;
      }
    }
  }
}
</style>
