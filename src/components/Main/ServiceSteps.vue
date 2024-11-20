<template>
  <div class="services-steps-block">
    <div class="container">
      <h2 class="title">Порядок оказания услуг</h2>
      <div class="steps__blocks">
        <div class="steps-list">
          <div class="list__item">
            <b>01</b>
            <p>Получение заявки и ваших пожеланий к уборке</p>
          </div>
          <div class="list__item">
            <b>02</b>
            <p>
              Озвучиваем примерную стоимость работ. Направляем оценщика на
              объект
            </p>
          </div>
          <div class="list__item">
            <b>03</b>
            <p>
              Осмотр помещения, точная оценка стоимости с учетом ваших пожеланий
            </p>
          </div>
          <div class="list__item">
            <b>04</b>
            <p>Делаем предложение с перечнем работ, их длительностью, ценой</p>
          </div>
          <div class="list__item">
            <b>05</b>
            <p>Проводим уборку на вашем обьекте</p>
          </div>
          <div class="list__item">
            <b>06</b>
            <p>Вы оплачиваете услуги</p>
          </div>
        </div>
        <div class="steps-img">
          <img src="/src/assets/steps_img.png" alt="" />
        </div>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.services-steps-block {
  h2.title {
    text-align: center;
    margin-bottom: 100px;
  }

  .steps__blocks {
    display: flex;
    position: relative;

    .steps-list {
      width: 50%;
      display: flex;
      flex-direction: column;
      margin-right: 51px;
    }

    .steps-img {
      width: 50%;
      background: #fff;
      padding: 34px 16px;
      height: 100%;
      display: flex;
      justify-content: center;
      align-items: center;
    }

    .list__item {
      padding: 20px 33px;
      background: #fff;
      display: flex;
      justify-content: start;
      align-items: center;
      margin-bottom: 26px;
      border-radius: 24px;

      b {
        background: rgba(#159bd6, 29%);
        width: 44px;
        height: 44px;
        display: flex;
        justify-content: center;
        align-items: center;
        border-radius: 50%;
        color: #159bd6;
        margin-right: 25px;
      }

      p {
        font-size: 17px;
        font-weight: 600;
        width: 80%;
      }
    }
  }
}
</style>
