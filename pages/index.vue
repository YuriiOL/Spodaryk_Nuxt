<template>
  <div>
    <main-banner />
    <info-block
      :link="{
        url: '/about',
        name: 'Про нас'
      }"
      :images="'/images/6.jpg'"
    >
      <template slot="mainTitle">
        Spodaryk Group
      </template>
      <template slot="smallTitle">
        Індивідуальний підхід у створенні унікального стилю вашого закладу
      </template>
      <template slot="text">
        Марія Сподарик - засновник та головна рушійною сила компанії Spodaryk Group
        Компанія почала свою діялність з 2009 року, Марія встигла попрацювати із відомою сіткою готелів
        <a href="" class="link">@reikartz_hotel_group</a> , ресторанами <a href="" class="link">@stargorodlviv</a> , <a
          href=""
          class="link"
        >@stargorod_dnepr</a> ,
        <a href="" class="link">@panskacharka</a> , «Дель Песто»,
        <a href="" class="link">@brudershaftlviv</a> , <a href="" class="link">@bagrationi_lviv</a> і з багатьма іншими
        відомими вітчизняними закладами...
      </template>
    </info-block>
    <regular-banner
      :main-title="'The latest'"
      :regular-title="'DESIGN'"
      :image="'linear-gradient(to bottom, rgba(0, 0, 0, 0.35), rgba(0, 0, 0, 0.55)), url(/_nuxt/static/images/bg-black-plane.jpg);'"
    />
    <info-block
      :link="{
        url: 'https://drive.google.com/drive/folders/1mE8kzWJpIlVwu0mu1M4LE89OqG5H-bcF',
        name: 'Каталог'
      }"
      :revers="true"
      :images="'/images/3.jpg'"
    >
      <template slot="mainTitle">
        Porcelain
      </template>
      <template slot="smallTitle">
        Фарфор
      </template>
      <template slot="text">
        Фарфор - витонченість, краса, класичні форми. Першокласна якість. Екологічність і безпека для здоров'я. Ідеальна
        глазурована поверхня. Здатність зберігати тепло. Стійкість до агресивних миючих засобів. Стійкість до механічних
        впливів при обробці в посудомийній машині. Зручність штабелювання і складування. Несхильність до старіння.
      </template>
    </info-block>
    <regular-banner
      :main-title="'The latest'"
      :regular-title="'DESIGN'"
      :image="'linear-gradient(to bottom,rgba(0,0,0,.35),rgba(0,0,0,.55)),url(../images/planes.jpg)'"
    />
    <bennefits />
  </div>
</template>
<script>
import MainBanner from '~/components/banners/main-banner'
import InfoBlock from '~/components/home/info-block'
import RegularBanner from '~/components/banners/regular-banner'
import Bennefits from '~/components/home/bennefits'

export default {
  components: {
    Bennefits,
    RegularBanner,
    InfoBlock,
    MainBanner
  },
  data: () => ({})
}
</script>
