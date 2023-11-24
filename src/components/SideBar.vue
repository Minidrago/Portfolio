<template lang="">
    <div class='sidebar'>
        <div @click="moveTo">
            <img class='/' src="../assets/icon/Home.png" alt="Home" title="Home">
        </div>
        <div @click="moveTo">
            <img class='about' src="../assets/icon/User.png" alt="About Me" title="About Me">
        </div>
        <div @click="moveTo">
            <img class='project' src="../assets/icon/Group of Projects.png" alt="Projects" title="Projects">
        </div>
        <div @click="moveTo">
            <img class='contact' src="../assets/icon/Gmail Logo.png" alt="Contact" title="Contact">
        </div>
    </div>
</template>
<script>
export default {
    name:"SideBar",
    methods:{
        moveTo(e){
            console.log(e.target.classList);
            let className = e.target.classList;
            this.$router.push(`/${className}`);
        }
    }
}
</script>
<style lang="scss">
    .sidebar{
        position: fixed;
        top: 0;
        right: 0;
        width: 4.5rem;
        height: 100vh;
        background-color: #E2E4E5;
        z-index: 9999;
        // position: absolute;
        div:nth-of-type(1){
            margin: 10vh auto;
            margin-bottom: 6vh;
            width: 50px;
            height: 50px;
            cursor: pointer;
            >img{width: 100%;}
        }
        div:nth-of-type(2){
            margin: 0 auto;
            width: 50px;
            height: 50px;
            cursor: pointer;
            >img{width: 100%;}
        }
        div:nth-of-type(3){
            margin: 0 auto;
            margin-top: 6vh;
            width: 50px;
            cursor: pointer;
            height: 50px;
            >img{width: 100%;}
        }
        div:nth-of-type(4){
            margin: 48vh auto;
            width: 50px;
            cursor: pointer;
            height: 50px;
            >img{width: 100%;}
        }
    }
</style>