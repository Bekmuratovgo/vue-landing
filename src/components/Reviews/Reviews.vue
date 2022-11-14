<template>
    <div class="reviews">
        <h2>Отзывы</h2>
        <div class="reviews_inner">
            <div class="btnGroup">
                <button class="btnReview">Видеоотзывы</button>
                <button class="btnReview">Текстовые отзывы</button>
                <button class="btnReview">Фотоотзывы</button>
                <p class="review-desc">Повышайте качество и эффективность работы Вашего бизнеса вместе с нами</p>
                <button class="tryFree">Попробовать бесплатно</button>
            </div>
            <div class="video">
                <div class="video_inner_left">
                    <img src="../../assets/img/video.png">
                </div>
                <div class="video_inner_right">
                    <img src="../../assets/img/miniVideo.png">
                    <img src="../../assets/img/miniVideo.png">
                    <img src="../../assets/img/miniVideo.png">
                </div>
                <img class="videoBgImg" src="../../assets/img/videoBgImg.png">
            </div>
        </div>
        <div>

        </div>
    </div>
</template>
  
<script>

export default {
    name: 'Reviews-Component',
    components: {
    }
}
</script>
  
<style>
.reviews {
    width: 100%;
    margin-top: 160px;
}

.reviews h2 {
    font-weight: 600;
    font-size: 25px;
}

.btnReview {
    font-size: 15px;
    border: none;
    border-radius: 50px;
    padding: 14px 19px;
    color: #B1ACC1;
    background: #F0F9FF;
    width: 270px;
    margin: 9px;
}

.reviews_inner {
    display: flex;
    justify-content: space-between;
}

@media screen and (max-width: 743px) {
    .reviews_inner {
        display: flex;
        justify-content: center;
        align-items: center;
        flex-direction: column-reverse;
    }
}

.review-desc {
    font-size: 15px;
    margin: 70px 0 28px;
    text-align: left;
}

.btnReview:hover {
    background: #FFD86B;
    transition: 0.3s;
    color: black;
}

.btnGroup {
    display: flex;
    flex-direction: column;
    align-items: center;
    width: 30%;
}

.tryFree {
    font-size: 15px;
    border: none;
    border-radius: 50px;
    padding: 14px 19px;
    color: white;
    background: #42B1F4;
}

.video {
    display: flex;
    width: 60%;
    position: relative;
}

.video_inner_left img {
    width: 100%;
}

.video_inner_right {
    display: flex;
    flex-direction: column;
    margin: 0 10px;
}

.video_inner_right img {
    width: 100%;
    margin: 0 0 8px;
}

.videoBgImg {
    position: absolute;
    right: -70px;
    top: -50px;
    z-index: -1;
    width: 115%;
}
</style>
  