<template>
    <div class="cardPercent">

        <h2> <img class="titleImg" src="../../assets/img/titleImg.png" alt=""> {{ componentTitle }}</h2>
        <p v-if="componentNumber === 2">JOBTRON поможет каждому сотруднику компании оценить свои силы и почувствовать
            поддержку. Благодаря нашей платформе каждый новый работник:</p>

        <div class="cardPercent_inner">
            <div class="cardItems" v-for="item in card" :class="item.bg" :key="item.bg">
                <h3 :class="item.bg">{{ item.title }}</h3>
                <h5 class="desc">{{ item.desc }}</h5>
            </div>
        </div>
        <div v-if="componentNumber === 2" class="inputWithBtn">
            <div class="inputWithBtn_inner">
                <h5>Повышайте качество и эффективность <br /> работы Вашего бизнеса вместе с нами</h5>
            </div>
            <div class="inputWithBtn__input">
                <input placeholder="Ваше имя" type="text">
                <input placeholder="Номер телефона" type="text">
            </div>
            <div class="cardBtnTryFree_wrapper">
                <button class="cardBtnTryFree">Попробовать бесплатно</button>
            </div>
        </div>
    </div>

</template>
  
<script>
export default {
    name: 'CardPercent-Component',
    components: {
    },
    props: {
        card: Array,
        componentTitle: String,
        componentNumber: Number,
    },
    data() {
        return {
        }
    },
}
</script>
  
<style>
.cardPercent {
    margin-top: 160px;
}

.blue {
    background: #EDF8FF;
    color: #72c6f9;
    margin: 10px 0;
    font-size: 38px;
}

.yellow {
    font-size: 38px;
    margin: 10px 0;
    background: #FFF9EA;
    color: #ffd86b;
}

.purpleBg {
    font-size: 38px;
    margin: 10px 0;
    background: #F3F0FC !important;
    color: #9082bb !important;
}

.desc {
    font-size: 15px;
    font-weight: 400;
    color: black;
    margin: 0;
    padding: 0 10px;
}

.cardPercent_inner {
    display: flex;
    justify-content: space-around;
    flex-wrap: wrap;
}

.inputWithBtn {
    display: flex;
    justify-content: space-around;
    margin-bottom: 50px;
    flex-wrap: wrap;
    /* text-align: left; */
}

.cardPercent h2 {
    font-weight: 600;
    font-size: 25px;
    margin: 0 0 0px 0;
    display: flex;
    align-items: center;
    justify-content: center;
    background-size: contain;
    height: 100px;
}

.cardItems {
    width: 270px;
    height: 240px;
    display: flex;
    flex-direction: column;
    justify-content: center;
    align-items: center;
    border-radius: 15px;
}

.cardBtnTryFree {
    font-size: 15px;
    border: none;
    border-radius: 50px;
    padding: 14px 19px;
    color: white;
    background: #42B1F4;
}

.inputWithBtn_inner h5 {
    font-weight: 400;
    margin: 0;
}
.inputWithBtn_inner {
    display: flex;
    align-items: center;
}

.inputWithBtn__input input {
    border: 1px solid #D9D9D9;
    border-radius: 15px;
    margin: 10px 0;
    padding: 14px 19px;
}

.titleImg {
    width: 100px;
    margin-right: -50px;
}
.cardBtnTryFree_wrapper {
    display: flex;
    align-items: center;
}
</style>
  