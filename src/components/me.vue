<template>
	<div class="aboutMe" @click="showMe">
                 <img src="../assets/image/me.png" alt="" class="me">
                 <img src="../assets/image/next.png" alt="" class="next">              
      </div>
      <transition name="fade">
            <div class="mask" v-show="isAbout"></div>                       
      </transition>
      <transition name="slide">
        <div class="about" v-if="isAbout" >
            <span class="close" @click="back">X</span>
            <div class="title">关于</div>
            <div class="name">XIEBING</div>
            <div class="job">求职意向: <span class="jobWanted">web前端工程师</span></div>
            <div>
                <p class="skill">技术栈:</p>
                <span class="skillDetail">
                    【前端】HTML/HTML5   CSS/CSS3   JavaScript(ES6,ES5)   SASS   Stylus   Vue.JS    微信小程序   Babel</br>
                    【后端】Node.js (express)</br>
                    【数据库】MongoDB</br>
                    【自动化构建】Webpack</br>
                    【版本管理】git
                </span>
            </div>
        </div>
      </transition>
</template>

<script>
	
</script>

<style lang="scss" scoped>
	@import '../assets/css/show.scss';
	
</style>
