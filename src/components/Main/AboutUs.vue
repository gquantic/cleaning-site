<template>
  <div class="about-us-block">
    <div class="container">
      <div class="about-us__items">
        <div class="about-us__description">
          <h2 class="title">О нас</h2>
          <div class="description__block">
            <ul>
              <li>
                8 лет на рынке клининговых услуг. <br />
                Отлаженный рабочий процесс
              </li>
              <li>
                20 сотрудников (4 бригады) в штате. <br />
                Тщательно отбираем персонал
              </li>
              <li>Используем дорогие экологичные моющие средства</li>
              <li>
                Все объекты, на которых мы проводим уборку, могут быть
                застрахованы
              </li>
              <li>
                Оплата после уборки. <br />
                Мы уверены в качестве своих работ
              </li>
              <li>Возможна уборка в день обращения</li>
            </ul>
          </div>
        </div>
        <img src="/src/assets/about_us_img.png" alt="" />
      </div>
    </div>
  </div>
</template>

<style lang="scss">
.about-us__items {
  display: flex;
  margin: 0 auto;
  width: fit-content;

  li::marker {
    display: none;
  }

  li {
    list-style: none;
    display: flex;
    align-items: center; // Центровка по вертикали
    position: relative;

    &::before {
      content: '';
      display: inline-block;
      width: 7px;
      height: 7px;
      background: inherit;
      border: 2px solid #000;
      border-radius: 50%;
      margin-right: 8px; // Отступ между точкой и текстом
      flex-shrink: 0; // Точка не сжимается
      margin-left: -30px;
      margin-right: 20px;
    }
  }

  h2.title {
    text-align: center;
  }

  .description__block {
    width: 636px;
    background: #fff;
    padding: 18px 30px;
    margin-right: -60px;
    position: relative;
    z-index: 2;

    li {
      font-size: 20px;
      font-weight: 500;
      margin-bottom: 23px;
    }
  }
}
</style>
