<template lang="">
    
    <div class="about">
        <div class="photo">
            <img src="../assets/img/profile.jpg">
        </div>
        <hr>
        <p>
            조금 늦은 출발이지만 열정과 꾸준함으로<br>새로운 기술과 도전을 두려워하지 않고 끊임없이 배우며 한걸음씩 나아가려고 합니다.<br>
            모나지 않은 둥글둥글한 성격으로 남들과 두루 어울리는걸 좋아하며,<br> 함께 협업하는게 즐거운 개발자를 목표로 하고 있습니다.
        </p>
        <h2 class='aboutme'>ABOUT ME</h2>
        <hr>
        <div class='aboutdetail'>
            <div class='detail1'>
                <figure>
                    <img src="../assets/icon/me.png">
                    <div>
                        <p>이름</p>
                        <p>조자룡</p>
                    </div>
                </figure>
                <figure>
                    <img src="../assets/icon/Party Hat.png">
                    <div>
                        <p>생년월일</p>
                        <p>86.01.10</p>
                    </div>
                </figure>
                <figure>
                    <img src="../assets/icon/Address.png">
                    <div>
                        <p>주소</p>
                        <p>서울시 강남구</p>
                    </div>
                </figure>
            </div>
            <div class='detail2'>
                <figure>
                    <img src="../assets/icon/iPhone SE.png">
                    <div>
                        <p>연락처</p>
                    <p>010-7371-6918</p>
                    </div>
                </figure>
                <figure>
                    <img src="../assets/icon/Email.png">
                    <div>
                        <p>이메일</p>
                    <p>socoool2@gmail.com</p>
                    </div>
                </figure>
            </div>
        </div>
        <h2 class='skill'>SKILLS</h2>
        <hr>
        <div class='skills'>
            <ul>
                <li>
                    <h2 class='frontend'>FRONTEND</h2>
                    <div class='imgs1'>
                        <div>
                            <img src="../assets/skill/Html.png">
                        </div>
                        <div>
                            <img src="../assets/skill/css.png">
                        </div>
                        <div>
                            <img src="../assets/skill/js.png">
                        </div>
                        <div>
                            <img src="../assets/skill/sass.png">
                        </div>
                        <div>
                            <img src="../assets/skill/react.png">
                        </div>
                        <div>
                            <img src="../assets/skill/next.png">
                        </div>
                        <div>
                            <img src="../assets/skill/vue.png">
                        </div>
                    </div>
                </li>

                <li>
                    <h2 class='database'>DATABASE</h2>
                    <div class='imgs2'>
                        <div>
                            <img src="../assets/skill/sql.png">
                        </div>
                        <div>
                            <img src="../assets/skill/mongodb.png">
                        </div>
                    </div>
                </li>

                <li>
                    <h2 class='tools'>TOOLS</h2>
                    <div class='imgs3'>
                        <div>
                            <img src="../assets/skill/vscode.png">
                        </div>
                        <div>
                            <img src="../assets/skill/github.png">
                        </div>
                        <div>
                            <img src="../assets/skill/git.png">
                        </div>
                    </div>
                </li>
            </ul>
        </div>
    </div>
</template>
<script>
export default {

}
</script>
<style lang="scss">
    .about{
        .photo{
            width: 30%;
            margin: 0 auto;
            padding-top: 5rem;
            >img{
                width: 100%;
            }
        }
        hr{
            margin: 5%;
            width: 85%;
            &:nth-of-type(2){
                width: 20%;
                transform: translateX(175%);
                margin-top: 1%;
            }
            &:nth-of-type(3){
                width: 20%;
                transform: translateX(175%);
                margin-top: 1%;
            }
        }
        p{
            font-size: 1.8rem;
            text-align: center;
            margin: 0 20%;
        }
        .aboutme{
            font-size: 4rem;
            text-align: center;
            margin: 5%;
            margin-bottom: 0;
        }
        .aboutdetail{
            .detail1{
                display: flex;
                // align-items: center;
                justify-content: center;
                >figure{
                    display: flex;
                    width: 15rem;
                    >img{
                        width: 4rem;
                        height: 4rem;
                        background-color: white;
                        border-radius: 1rem;
                    }
                    >div{
                        p:nth-of-type(1){
                            font-size: 1.5rem;
                            width: 100%;
                            margin: 0 1rem;
                            text-align: left;
                        }
                        p:nth-of-type(2){
                            font-size: 1.4rem;
                            width: 100%;
                            margin: 1rem;
                            text-align: left;
                        }
                    }
                }
            }
            .detail2{
                display: flex;
                // align-items: center;
                justify-content: center;
                >figure{
                    display: flex;
                    width: 15rem;
                    >img{
                        width: 4rem;
                        height: 4rem;
                        background-color: white;
                        border-radius: 1rem;
                    }
                    >div{
                        p:nth-of-type(1){
                            font-size: 1.5rem;
                            width: 100%;
                            margin: 0 1rem;
                            text-align: left;
                        }
                        p:nth-of-type(2){
                            font-size: 1.4rem;
                            width: 100%;
                            margin: 1rem;
                            text-align: left;
                        }
                    }
                }
            }
        }
        .skill{
            font-size: 4rem;
            text-align: center;
            margin: 5%;
            margin-bottom: 0;
        }
        .skills{
            ul{
                li:nth-of-type(1){
                    
                    .frontend{
                        text-align: center;
                    }
                    .imgs1{
                        display: flex;
                        background-color: white;
                        height: 100%;
                        justify-content: center;
                        align-items: center;
                        width: 35rem;
                        margin: 0 auto;
                        img{
                            margin: 1rem 1rem;
                        }
                    }
                }
                li:nth-of-type(2){
                    
                    .database{
                        margin: 2rem;
                        text-align: center;
                    }
                    .imgs2{
                        display: flex;
                        background-color: white;
                        height: 100%;
                        justify-content: center;
                        align-items: center;
                        width: 35rem;
                        margin: 0 auto;
                        img{
                            margin: 1rem 1rem;
                        }
                    }
                }
                li:nth-of-type(3){
                    
                    .tools{
                        margin: 2rem;
                        text-align: center;
                    }
                    .imgs3{
                        display: flex;
                        background-color: white;
                        height: 100%;
                        justify-content: center;
                        align-items: center;
                        width: 35rem;
                        margin: 0 auto;
                        img{
                            margin: 1rem 1rem;
                        }
                    }
                }
            }
        }
    }
    
</style>