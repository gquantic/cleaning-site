<script>
import { ref } from 'vue'

const services = ref('')
const selectedService = ref('')

services.value = [
  {
    title: 'Уборка после ремонта',
    priceForRoom: 1000,
  },
]
</script>

<template>
  <div class="calc-block">
    <div class="container">
      <h2>Рассчитайте стоимость уборки</h2>

      <div class="calc">
        <div>
          <div class="form-group mt-3">
            <label>Количество комнат</label>
            <div class="select-rooms">
              <button class="selected">1</button>
              <button>2</button>
              <button>3</button>
              <button>4</button>
              <button>5+</button>
            </div>
          </div>
          <div class="form-group mt-3">
            <label>Тип уборки</label>
            <select
              name=""
              id=""
              class="form-input mt-1"
              v-model="selectedService"
            >
              <option
                value=""
                v-for="(service, index) in services"
                :key="index"
              >
                {{ service.title }}
              </option>
            </select>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.calc-block {
  padding: 63px 0;
  background: #fff;
  width: 100%;

  h2 {
    font-size: 32px;
  }

  .select-rooms {
    display: flex;
    margin-top: 14px;

    button {
      width: 57px;
      height: 57px;
      margin-right: 15px;
      border: none;
      border-radius: 50%;
      background: rgba(#159bd6, 0%);
      transition: 0.3s ease;
      font-size: 20px;
      font-family: 'Montserrat', Arial;
      font-weight: 600;

      &.selected {
        background: #159bd6;
        color: #fff;
      }
    }
  }
}
</style>
