<script setup>
import { ref, onMounted } from 'vue';
onMounted(()=>{
    const slides = document.querySelector('.slides')
    const slide = document.querySelectorAll('.slide')
    const prev = document.querySelector('.prev')
    const next = document.querySelector('.next')
    let index = 0
    const totalSlides = slide.length
    const slideWidth = slide[0].clientWidth

    next.addEventListener('click', () => {
        index++
        if (index >= totalSlides) {
            index = 0
        }
        updateSlide()
    })

    prev.addEventListener('click', () => {
        index--
        if (index < 0) {
            index = totalSlides - 1
        }
        updateSlide()
    })

    function updateSlide() {
        slides.style.transform = `translateX(-${index * slideWidth}px)`
    }
});
</script>

<template>
	<div class="container">
        <div class="container-inner">
            <div class="landing-block">
                <div class="landing-block__slider landing-block_box">
                    <div class="slider-container">
                        <div class="slides">
                            <div class="slide">
                                <img class="slider-img__first" src="../public/image/sliderNumbers.png" alt="#" />
                                <img src="../public/image/sliderText.png" alt="#">
                            </div>
                            <div class="slide">
                                <img class="slider-img__first" src="../public/image/sliderNumbers.png" alt="#" />
                                <img src="../public/image/sliderText.png" alt="#">
                            </div>
                        </div>
                        <button class="btn prev"><img src="../public/image/arrow.svg" alt="#"></button>
                        <button class="btn next"><img src="../public/image/arrow.svg" alt="#"></button>
		            </div>
                </div>
                <div class="landing-block__news_free-del landing-block_box">
                    <div class="news_free-del__text">
                        <img class="textImg" src="../public/image/deliveryTextImg.png" alt="#">
                        <img class="line" src="../public/image/vectorLine.svg" alt="#">
                    </div>
                    <img class="free-del-manImg" src="../public/image/manImg.png" alt="#">
                </div>
                <div class="landing-block__news-fees landing-block_box">
                    <div class="news-fees__text">
                        <img class="textImg2" src="../public/image/feeImgText.png" alt="#">
                        <img class="line2" src="../public/image/vector2.png" alt="#">
                    </div>
                    <img class="news-fees__manImg" src="../public/image/mainImg2.png" alt="#">
                </div>
                <div class="landing-block__book landing-block_box">
                    book
                </div>
            </div>
        </div>
	</div>
</template>

<style lang="scss" scoped>
    .container{
        padding: 0px;
		display: flex;
		align-items: center;
		justify-content: center;
		margin: 0 auto;
		width: 1366px;
        background-color: #F9F9FA;
    }
    .container-inner{
		width: calc(100% - 226px);
        margin-top: 30px;
	}
    .landing-block{
        width: 100%;
        height: 520px;
        display: grid;
        grid-template-columns: 360px 360px 360px;
        grid-template-rows: 350px 140px;
        grid-auto-flow: row dense;
        gap: 30px;
        grid-template-areas: "s s b"
                             "f fe b";
    }
    .landing-block_box{
        border-radius: 5px;
        width: 100%;
        background-color: red;
        overflow: hidden;
        display: flex;
        align-items: center;
    }
    .landing-block__slider{
        grid-column: span 2;
        grid-area: s;
    }
    .landing-block__news_free-del{
        grid-area: f;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0 25px;
        background-color: #6D378F;
    }
    .landing-block__news-fees{
        grid-area: fe;
        display: flex;
        align-items: center;
        justify-content: space-between;
        padding: 0 25px;
        background-color: #FFD8EF;
    }
    .landing-block__book{grid-area: b;}
    .slider-container {
        width: 100%;
        height: 100%;
        overflow: hidden;
        position: relative;
    }
    .slides {
        width: 100%;
        height: 100%;
        display: flex;
        transition: transform 0.5s ease-in-out;
    }
    .slide {
        min-width: 100%;
        height: 100%;
        text-align: center;
        padding: 50px 0;
        display: flex;
        align-items: center;
        justify-content: center;
        flex-direction: column;
        background-color: #CCFF90;
    }
    .slider-img__first{
        margin-bottom: 20px;
    }
    .btn {
        position: absolute;
        width: 40px;
        height: 40px;
        display: flex;
        align-items: center;
        background-color: #FFFFFFD9;
        justify-content: center;
        cursor: pointer;
        border-radius: 5px;
        top: calc(50% - 20px);
    }
    .next{
        transform: rotate(180deg);
        right: 27px;
    }
    .prev{
         left: 27px;
    }
    .news_free-del__text{
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
    }
    .line{
        position: absolute;
        top: -5px;
        left: -12px;
    }
    .line2{
        position: absolute;
        bottom: -5px;
        left: 17px;
    }
    .free-del-manImg{
        width: 100px;
        height: 100px;
    }
    .textImg{
        z-index: 1;
    }
    .textImg2{
        z-index: 1;
    }
    .news-fees__text{
        position: relative;
        display: flex;
        align-items: center;
        justify-content: center;
    }
</style>
