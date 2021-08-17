<template>
  <div class="about-info-container">
    <div class="about-info">
      <h1 class="about-info__title">
        Індивідуальний підхід у створенні унікального стилю вашого закладу
      </h1>
      <p class="about-info__text">
        Марія Сподарик - засновник та головна рушійною сила компанії Spodaryk Group
        Компанія почала свою діялність з 2009 року, Марія встигла попрацювати із відомою сіткою готелів
        <a href="" class="link">@reikartz_hotel_group</a> , ресторанами <a href="" class="link">@stargorodlviv</a> , <a
          href=""
          class="link"
        >@stargorod_dnepr</a> ,
        <a href="" class="link">@panskacharka</a> , «Дель Песто»,
        <a href="" class="link">@brudershaftlviv</a> , <a href="" class="link">@bagrationi_lviv</a> і з багатьма іншими
        відомими вітчизняними закладами. Радує, що в Україні є
        такі
        люди, які приходять в бізнес не заради самого бізнесу, а усвідомлено, з особливою місією надавати якісні послуги
        і
        знаходити правильні рішення для підкреслення індивідуальності кожного закладу.
      </p>
      <p class="about-info__text">
        Отож, ціллю для Марії стало привнесення різноманітності, оригінальності та еталонної якості в ресторанну сферу.
        Вона
        добре знає, як важливо власнику закладу справити сприятливе враження на відвідувачів. На це впливає не тільки
        оригінальний стиль закладу, єдиний дизайн всіх елементів, але й ресторанний посуд, який є атрибутом будь-якого
        ресторанно-готельного комплексу.
      </p>
    </div>
  </div>
</template>

<script>
export default {}
</script>

<style scoped lang="scss">
.top-wrapper-about {
  margin-top: 80px;
  min-height: 50vh;
}

.about-info {
  padding: 50px 30px;

  &__title {
    @include small-title;
    text-align: center;
    margin-bottom: 20px;
    font-size: 30px;
  }

  &__text {
    @include about-regular-text;
  }
}

.link {
  @include links;
}
</style>
