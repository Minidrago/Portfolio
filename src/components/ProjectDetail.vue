<template lang="">
    <div class='detail'>
        <div class='arrow'>
            <router-link to="/project">
                <div>
                    <img src="../assets/icon/Left Arrow.png">
                </div>
                <p>List</p>
            </router-link>
        </div>
        <h1 v-for="item in jsonData[0].title" :key="item.id">{{item}}</h1>
        <P>{{jsonData[0].date}}</P>
        
        <div class='content'>
            <div class='images'>
                <figure>
                    <swiper
                        :spaceBetween="30"
                        :centeredSlides="true"
                        :autoplay="{
                        delay: 3000,
                        disableOnInteraction: false,
                        }"
                        :pagination="{
                        clickable: true,
                        }"
                        :navigation="true"
                        :modules="modules"
                        class="mySwiper3"
                    >
                        <swiper-slide>
                            <div v-for="item in jsonData[0].title" :key="item.id">
                                <img src="{{jsonData[0].images[0]}}">
                            </div>
                        </swiper-slide>
                        <swiper-slide>Slide 2</swiper-slide>
                    </swiper>
                    <div>
                        <img src="../assets/project/clone.png">
                    </div>
                    <figcaption>
                        <div>
                            <img src="../assets/icon/Chevron Left.png" alt="left">
                        </div>
                        <p>1/4</p>
                        <div>
                            <img src="../assets/icon/Chevron Right.png" alt="right">
                        </div>
                    </figcaption>
                </figure>
            </div>

            <div class='texts'>
                <p>코딩 시작 후...</p>
                <div class='look'>
                    <P>자세히 보기</P>
                    <div>
                        <img src='../assets/icon/Right Button.png'>
                    </div>
                    <div>
                        <img src='../assets/icon/github.png'>
                    </div>
                </div>
                
                <div class='check'>
                    <div>
                        <img src="../assets/icon/Check.png">
                        <p>주요기능</p>
                    </div>
                    <div>
                        <img src="../assets/icon/Check.png">
                        <p>GitHub</p>
                    </div>
                    <div>
                        <img src="../assets/icon/Check.png">
                        <p>URL</p>
                    </div>
                    <div>
                        <img src="../assets/icon/Check.png">
                        <p>Frontend</p>
                    </div>
                    <div>
                        <img src="../assets/icon/Check.png">
                        <p>Deployment</p>
                    </div>
                </div>
            </div>
        </div>
    </div>
</template>
<script>
import detaildb from "../json/detail.json";

//Swiper
import { Swiper, SwiperSlide } from 'swiper/vue';
// Import Swiper styles
import 'swiper/css';
import 'swiper/css/pagination';
import 'swiper/css/navigation';
import '../css/detail.css';
import { Autoplay, Pagination, Navigation } from 'swiper/modules';

export default {
    data() {
        return {
            jsonData: detaildb
        };
    },
    components: {
        Swiper,
        SwiperSlide,
    },
    setup() {
      return {
        modules: [Autoplay, Pagination, Navigation],
      };
    },
}
</script>
<style lang="scss">
    .detail{

        .arrow{
            position: absolute;
            top: 14%;
            left: 5%;
            border-bottom: 2px solid white;
            >a{
                display: flex;
                align-items: center;
                >div{
                    >img{width: 100%;}
                }
                >p{
                    color: white;
                    font-size: 2.25rem;
                    font-weight: 700;
                    margin:0;
                    margin-left: 3rem;
                }
            }
        }
        
        h1{
            font-size: 4rem;
            font-weight: 900;
            text-align: center;
            margin: 0;
            padding-top: 5rem;
        }
        >p{
            font-size: 1.5rem;
            text-align: center;
            color: #B7BCC0;
        }

        .content{
            display: flex;
            justify-content: space-between;
            margin-top: 3%;
            
            .images{
                width: 46%;
                >figure{
                    >div{
                        >img{width: 100%;}
                    }
                    >figcaption{
                        display: flex;
                        justify-content: center;
                        align-items: center;
                        >div:nth-last-of-type(1){
                            width: 4.5%;
                            >img{width: 100%;}
                        }
                        >p{
                            font-size: 2rem;
                            margin: 0;
                        }
                        >div:nth-last-of-type(2){
                            width: 4.5%;
                            >img{width: 100%;}
                        }
                    }
                }
            }

            .texts{
                width: 46%;
                >p{
                    font-size: 1.125rem;
                }
                .look{
                    >p{
                        font-size: 1.5rem;
                    }
                    >div:nth-of-type(1){
                        width: 1.5rem;
                        height: 1.5rem;
                        >img{width: 100%;}
                    }
                    >div:nth-of-type(2){
                        width: 1.5rem;
                        height: 1.5rem;
                        >img{width: 80%;}
                    }
                }
                
            }
        }
    }
</style>