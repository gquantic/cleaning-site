<template>
  <div class="wcc-block">
    <div class="container">
      <div class="title-block">
        <h2 class="title">Почему люди выбирают клининг?</h2>
        <img src="/src/assets/wcc_img.png" alt="" />
      </div>
      <div class="wcc-items">
        <div class="wcc-item">
          <img src="/src/svg/check.svg" alt="" />
          <div class="text">
            <p class="bold">Высокое качество уборки</p>
            <p>
              Наши профессионалы добиваются глубокой чистоты, недоступной при
              обычной уборке
            </p>
          </div>
        </div>

        <div class="wcc-item">
          <img src="/src/svg/file-text.svg" alt="" />
          <div class="text">
            <p class="bold">Специализированные знания и оборудование</p>
            <p>
              Профессиональное оборудование и навыки позволяют справляться даже
              с сильными загрязнениями
            </p>
          </div>
        </div>

        <div class="wcc-item">
          <img src="/src/svg/time.svg" alt="" />
          <div class="text">
            <p class="bold">Экономия времени</p>
            <p>
              Уборка отнимает много времени, и клининг позволяет сэкономить его
              для более важных дел
            </p>
          </div>
        </div>

        <div class="wcc-item">
          <img src="/src/svg/option.svg" alt="" />
          <div class="text">
            <p class="bold">Удобство</p>
            <p>
              Уборка проводится по удобному графику, можно выбрать разовый или
              регулярный вариант
            </p>
          </div>
        </div>

        <div class="wcc-item">
          <img src="/src/svg/x.svg" alt="" />
          <div class="text">
            <p class="bold">Экологичность</p>
            <p>Используются безопасные для здоровья и экологии средства</p>
          </div>
        </div>

        <div class="wcc-item">
          <img src="/src/svg/warning.svg" alt="" />
          <div class="text">
            <p class="bold">Безопасность</p>
            <p>
              Специалисты обучены безопасному обращению с химией и
              оборудованием, минимизируя риски
            </p>
          </div>
        </div>
      </div>

      <div class="btn-block">
        <button class="btn btn-primary">Заказать</button>
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.wcc-block {
  background: #fff;

  .btn-block {
    text-align: center;
    margin-top: 80px;
  }

  .title-block {
    display: flex;
    justify-content: space-between;

    h2 {
      margin-top: 110px;
      font-weight: 500;
      width: 393px;
    }

    img {
      margin-top: -60px;
    }
  }

  .wcc-items {
    display: flex;
    justify-content: space-between;
    flex-wrap: wrap;
    margin-top: 44px;

    .wcc-item {
      height: 108px;
      width: 581px;

      display: flex;
      justify-content: start;
      align-items: start;

      .text {
        margin-left: 33px;

        p.bold {
          margin-top: 0;
          margin-bottom: 12px;
          font-weight: 700;
          font-size: 20px;
        }

        p {
          margin: 0;
        }
      }
    }
  }
}
</style>
