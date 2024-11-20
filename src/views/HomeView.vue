<script setup lang="ts">
import CalcPrice from '@/components/CalcPrice.vue'
import AboutUs from '@/components/Main/AboutUs.vue'
import Services from '@/components/Main/Services.vue'
import ServiceSteps from '@/components/Main/ServiceSteps.vue'
import WhyChooseCleaning from '@/components/Main/WhyChooseCleaning.vue'
</script>

<template>
  <div class="container block-margin-bottom">
    <div class="first-block">
      <div>
        <h2>
          Клининг <br />
          в Краснодаре
        </h2>
        <p>Чистота быстро, качественно и не дорого</p>

        <div class="achievements-block">
          <div class="achievements">
            <div>
              <b>8</b>
              <p>лет на рынке</p>
            </div>
            <div>
              <b>40</b>
              <p>специалистов</p>
            </div>
            <div>
              <b>100+</b>
              <p>довольных клиентов</p>
            </div>
          </div>

          <div class="call-order-mask">
            <button class="call-order">звонок</button>
          </div>
        </div>
      </div>
      <img src="@/assets/block_first.webp" alt="" />
    </div>
  </div>
  <Services />
  <AboutUs />
  <ServiceSteps />
  <WhyChooseCleaning />
</template>
