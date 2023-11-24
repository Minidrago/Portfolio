<template lang="">
    <div class='background'>
        <div class='contact'>
            <h1>CONTACT</h1>
            <div class='text'>
                <P>010-3470-6918</P>
                <P>socoool2@gmail.com</P>
                <div>
                    <a href="https://github.com/Minidrago">
                        <img src="../assets/img/깃허브이미지.png">
                    </a>    
                </div>
            </div>
            
            
        </div>
    </div>
    <SideBar />
</template>
<script>
import SideBar from '@/components/SideBar.vue'

export default {
    components: {
    SideBar
}
}
</script>
<style lang="scss">
    #app{
        .background{
            .contact{
                display: flex;
                justify-content: center;
                gap: 10rem;
                padding-top: 15%;
                >h1{
                    font-size: 4rem;
                }
                .text{
                    p:nth-of-type(1){
                        font-size: 2.5rem;
                    }
                    p:nth-of-type(2){
                        font-size: 2.5rem;
                    }
                    >div{
                        width: 11.25rem;
                        height: 6rem;
                        a{
                            >img{
                                width: 100%;
                            }
                        }
                    }
                }
            }
        }
    }
</style>