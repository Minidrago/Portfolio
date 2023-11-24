<template>
    <SideBar />
    
    <div class="project">
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
        <router-link to="/detail">
            <div class="first">
                <p><span>Clone</span> 01</p>
                <h2>2022 SEOUL MUSIC<br> FESTIVAL</h2>
                <figure>
                    <div>
                        <img src="../assets/project/clone.png">
                    </div>
                    <p>
                        HTML, SCSS, JavaScript
                    </p>
                    <figcaption>
                        코딩 공부 시작 후 처음 진행해 본 프로젝트입니다.기본적인 HTML, CSS, JavaScript만을 사용하여 제작 하였으며, 이론으로 배우기만 했던 내용을 실제로 써보면서 코딩의 재미를 느낄 수 있게 해준 의미있는 프로젝트입니다.  
                    </figcaption>
                </figure>
            </div>
        </router-link>
      </swiper-slide>
    
      <swiper-slide>
        <router-link to="/detail">
            <div class="second">
                <p><span>Team</span> 02</p>
                <h2>ToEat</h2>
                <figure>
                    <div>
                        <img src="../assets/project/toeat.png">
                    </div>
                    <p>
                        HTML, SCSS, JavaScript
                    </p>
                    <figcaption>
                        코딩 공부 시작 후 처음 진행해 본 프로젝트입니다.기본적인 HTML, CSS, JavaScript만을 사용하여 제작 하였으며, 이론으로 배우기만 했던 내용을 실제로 써보면서 코딩의 재미를 느낄 수 있게 해준 의미있는 프로젝트입니다.  
                    </figcaption>
                </figure>
            </div>
      </router-link>
      </swiper-slide>
      
      <swiper-slide>
        <router-link to="/detail">
           <div class="third">
            <p><span>Single</span> 03</p>
            <h2>Mountain</h2>
            <figure>
                <div>
                    <img src="../assets/project/mountain.png">
                </div>
                <p>
                    HTML, SCSS, JavaScript
                </p>
                <figcaption>
                    코딩 공부 시작 후 처음 진행해 본 프로젝트입니다.기본적인 HTML, CSS, JavaScript만을 사용하여 제작 하였으며, 이론으로 배우기만 했던 내용을 실제로 써보면서 코딩의 재미를 느낄 수 있게 해준 의미있는 프로젝트입니다.  
                </figcaption>
            </figure>
           </div>
        </router-link>
      </swiper-slide>

      <swiper-slide>
        <router-link to="/detail">
            <div class="fourth">
                <p><span>Team</span> 04</p>
                <h2>JejePick</h2>
                <figure>
                    <div>
                        <img src="../assets/project/jejepick.png">
                    </div>
                    <p>
                        HTML, SCSS, JavaScript
                    </p>
                    <figcaption>
                        코딩 공부 시작 후 처음 진행해 본 프로젝트입니다.기본적인 HTML, CSS, JavaScript만을 사용하여 제작 하였으며, 이론으로 배우기만 했던 내용을 실제로 써보면서 코딩의 재미를 느낄 수 있게 해준 의미있는 프로젝트입니다.  
                    </figcaption>
                </figure>
            </div>
        </router-link>
      </swiper-slide>
    </swiper>
    </div>
</template>
<script>
import { Swiper, SwiperSlide } from 'swiper/vue';
import SideBar from '@/components/SideBar.vue'
import 'swiper/css';
import 'swiper/css/pagination';
import '../css/project.css';
import { Mousewheel} from 'swiper/modules';

export default {
    components: {
        SideBar,
        Swiper,
        SwiperSlide,
    },
    setup() {
        return {
            modules: [Mousewheel],
        };
    },
};
</script>
<style lang="scss"> 
    .project{
        
        .first{
            height: 100vh;
            margin-right: 10%;
            
            >p{
                text-align: right;
                color: white;
                padding-right: 1.5rem;
                font-size: 3.75rem;
                font-weight: 700;
                margin: 0;
                padding-top: 12%;
                >span{
                    font-size: 1.5rem;
                }
            }
            >h2{
                color: white;
                text-align: right;
                padding-right: 1.5rem;
                font-size: 2rem;
                margin-top: 20%;
            }
            >figure{
                margin: 0;
                >div{
                    width: 100%;
                    height: 19.25rem;
                    >img{
                    width: 100%;
                    }
                }
                >p{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
                >figcaption{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
            }
        }
        .second{
            height: 100vh;
            margin-right: 10%;

            >p{
                text-align: right;
                color: white;
                padding-right: 1.5rem;
                font-size: 3.75rem;
                font-weight: 700;
                margin: 0;
                padding-top: 12%;
                >span{
                    font-size: 1.5rem;
                }
            }
            >h2{
                color: white;
                text-align: right;
                padding-right: 1.5rem;
                font-size: 2rem;
                margin-top: 20%;
            }
            >figure{
                margin: 0;
                >div{
                    width: 100%;
                    height: 19.25rem;
                    >img{
                    width: 100%;
                }
                }
                >p{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
                >figcaption{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
            }
        }
        .third{
            height: 100vh;
            margin-right: 10%;

            >p{
                text-align: right;
                color: white;
                padding-right: 1.5rem;
                font-size: 3.75rem;
                font-weight: 700;
                margin: 0;
                padding-top: 12%;
                >span{
                    font-size: 1.5rem;
                }
            }
            >h2{
                color: white;
                text-align: right;
                padding-right: 1.5rem;
                font-size: 2rem;
                margin-top: 20%;
            }
            >figure{
                margin: 0;
                >div{
                    width: 100%;
                    height: 19.25rem;
                    >img{
                    width: 100%;
                }
                }
                >p{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
                >figcaption{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
            }
        }
        .fourth{
            height: 100vh;
            margin-right: 10%;

            >p{
                text-align: right;
                color: white;
                padding-right: 1.5rem;
                font-size: 3.75rem;
                font-weight: 700;
                margin: 0;
                padding-top: 12%;
                >span{
                    font-size: 1.5rem;
                }
            }
            >h2{
                color: white;
                text-align: right;
                padding-right: 1.5rem;
                font-size: 2rem;
                margin-top: 20%;
            }
            >figure{
                margin: 0;
                >div{
                    width: 100%;
                    height: 19.25rem;
                    >img{
                    width: 100%;
                }
                }
                >p{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
                >figcaption{
                    color: white;
                    text-align: right;
                    padding-right: 1.5rem;
                }
            }
        }
    }
</style>


