<template>
  
  <div class="home">
    <Vue3Typer  text="프론트엔드 개발자 조자룡의 포트폴리오 입니다." pre-type-delay='2000' type-delay='110' />
    
    <div class="figure">
      <swiper
      :scrollbar="{
        hide: true,
      }"
      :slidesPerView="3"
      :centeredSlides="true"
      :mousewheel="true"
      :modules="modules"
      class="mySwiper">
    
      <swiper-slide>
        <router-link to="/about">
        <figure class="ab">
            <img src="../assets/img/about.png">
            <figcaption>About me</figcaption>
            <p>안녕하세요! 주니어 개발자입니다!</p>
          </figure>
        </router-link>
      </swiper-slide>
    
      <swiper-slide>
        <router-link to="/project">
        <figure>
          <img src="../assets/img/project.png">
          <figcaption>Portfolio</figcaption>
          <p>한걸음씩 나아가는 프로젝트 모음집입니다!</p>
        </figure>
      </router-link>
      </swiper-slide>
      
      <swiper-slide>
        <router-link to="/contact">
        <figure>
          <img src="../assets/img/contact.png">
          <figcaption>Contact</figcaption>
          <p>문의나 제안이 있으신가요? 언제든지 연락 주세요!</p>
        </figure>
      </router-link>
      </swiper-slide>

      </swiper>
    </div>
    <SideBar />
  </div>
  
</template>
<script>
import Vue3Typer from 'vue3-typer'
import '../css/typer.css'
import SideBar from '@/components/SideBar.vue'

import { Swiper, SwiperSlide } from 'swiper/vue';
import { Mousewheel} from 'swiper/modules';
import 'swiper/css';
// import { Scrollbar } from 'swiper/modules';
// import 'swiper/css/scrollbar';

export default {
  el: "#app",
  name: 'HomeView',
  components: {
    SideBar,
    Vue3Typer,
    Swiper,
    SwiperSlide,
  },
  setup() {
      return {
        modules: [Mousewheel],
      };
  },

}
</script>

<style lang="scss">
// .swiper-scrollbar {
//   background-color: rgba(255,255,255,0.4);
// }
// .swiper-scrollbar-drag{
//   background-color: #eee;
// }
.swiper-slide {
  transition: 1s;
}
// .swiper-wrapper{padding: 3% 0 !important;}
.swiper-slide-active{
  transform: translateY(12%) !important;
}
  .home{
    .vue-typer{
      margin-top: 0;
      padding-top: 5rem;
    }
    p{
      color: white;
      z-index: 10;
    }
    .figure{
      margin-left: 10rem;

      figure{
        position: relative;
        color: white;
        margin: 5rem;
        transform: translateX(-20%);
        width: 80%;
        img{
          width: 100%;
        }
        figcaption{
          position: absolute;
          top: 0;
          right: 0;
          color: #D2074A;
          font-size: 2.5rem;
          font-weight: bold;
        }
        p{
          position: absolute;
          bottom: 0;
          right: 50%;
          transform: translateX(50%);
          font-size: 1.5rem;
          font-weight: 500;
          display: none;
        }
      }
      figure::before {
        content: "";
        position: absolute;
        top: 0;
        left: 0;
        width: 100%;
        height: 100%;
        transition: 0.5s;
      }
      figure:hover::before {
        background-color: #D2074A;
        opacity: 80%;
      }
      figure:hover{
        figcaption{color: white;}
        p{display: block;}
      }
      
      
    }
  }
</style>
