<template>
    <div class="main">
        <div class="main_inner">
            <div class="main_inner__body">
                <h2>JOBTRON: удобно для сотрудников, полезно для бизнеса</h2>
                <div class="mainNavbar">
                    <div class="mainNavbar_inner">
                        <div class="questionWrapper">
                            <h5>Личный профиль</h5>
                            <div class="question"><img src="../assets/img/_.png" /></div>
                        </div>
                        <div class="questionWrapper">
                            <h5>База знаний</h5>
                            <div class="question"><img src="../assets/img/_.png" /></div>
                        </div>
                        <div class="questionWrapper">
                            <h5>KPI</h5>
                            <div class="question"><img src="../assets/img/_.png" /></div>
                        </div>
                        <div class="questionWrapper">
                            <h5>Курсы</h5>
                            <div class="question"><img src="../assets/img/_.png" /></div>
                        </div>
                        <div class="questionWrapper">
                            <h5>Структура компании</h5>
                            <div class="question"><img src="../assets/img/_.png" /></div>
                        </div>
                        <div class="questionWrapper">
                            <h5>Новости и чат</h5>
                            <div class="question"><img src="../assets/img/_.png" /></div>
                        </div>
                    </div>
                </div>
                <div class="main_inner__tableBlock">
                    <div class="descriptionBlock_wrapper">
                        <div class="descriptionBlock">
                            <h4>Полезно для сотрудника: </h4>
                            <h5> <img class="dots" src="../assets/img/dots.png"> все заработанные деньги видны на экране
                            </h5>
                            <h5> <img class="dots" src="../assets/img/dots.png"> % выполнения KPI в реальном времени
                            </h5>
                            <h5> <img class="dots" src="../assets/img/dots.png"> премии, бонусы, электронные награды и
                                сертификаты</h5>
                            <h5> <img class="dots" src="../assets/img/dots.png"> оценка эффективности собственной работы
                            </h5>
                        </div>
                        <div class="descriptionBlock" style="margin-top: 37px">
                            <h4>Полезно для руководителей:</h4>
                            <h5> <img class="dots" src="../assets/img/dots.png"> повышение эффективности каждого
                                сотрудника
                            </h5>
                            <h5> <img class="dots" src="../assets/img/dots.png">много инструментов мотивации персонала
                            </h5>
                            <h5> <img class="dots" src="../assets/img/dots.png"> увеличение вовлеченности</h5>
                            <h5> <img class="dots" src="../assets/img/dots.png"> цифровые SMART цели
                            </h5>
                        </div>
                        <button class="getFreeBtn">Получить бесплатно</button>
                    </div>
                    <div class="tableBlock_wrapper">
                        <img class="tableImg" src="../assets/img/table.png">
                    </div>
                </div>
                <div></div>
            </div>
            <CardPercent :card="card1" :componentNumber="1"
                :componentTitle="'Компании, использующие JOBTRON, отмечают:'" />
            <Reviews />
            <Rates />
            <WorkJobTron />
            <CardPercent :card="card2" :componentNumber="2" :componentTitle="'JOBTRON в цифрах'" />
        </div>
        <img class="bg-left" src="../assets/img/bg-left.png" alt="">
        <img class="bg-right" src="../assets/img/bg-right.png" alt="">

    </div>
</template>
  
<script>
import CardPercent from '@/components/CardPercent/CardPercent.vue';
import Rates from '@/components/Rates/Rates.vue';
import Reviews from '@/components/Reviews/Reviews.vue';
import WorkJobTron from '@/components/WorkJobTron/WorkJobTron.vue';

export default {
    name: 'Main-Page',
    components: {
        CardPercent,
        Reviews,
        WorkJobTron,
        Rates
    },
    data() {
        return {
            card1: [
                { bg: 'blue', title: 'на 29 %', desc: 'Снизилась текучка сотрудников' },
                { bg: 'yellow', title: 'на 15 %', desc: 'Увеличилось число активных работников, предлагающих нестандартные решения' },
                { bg: 'purpleBg', title: 'на 25 %', desc: 'Увеличилось вовлеченность сотрудников в жизнь компании' },
            ],
            card2: [
                { bg: 'blue', title: '3', desc: 'В 3 раза быстрее адаптируется к работе в компании' },
                { bg: 'yellow', title: 'на 21 %', desc: 'Повышает свою продуктивность' },
                { bg: 'purpleBg', title: 'на 22 %', desc: 'Повышает свой доход уже через два месяца после начала рбаоты' },
            ],
        }
    },
}
</script>
  
<style>
.main {
    position: relative;
    display: flex;
    justify-content: center;
    width: 100%;
}

.main_inner {
    width: 80%;
    margin-top: 51px;
}

.main_inner__body h2 {
    font-weight: 600;
    font-size: 25px;
    margin: 0;
}

.mainNavbar {
    margin-top: 53px;
    display: flex;
    justify-content: center;
}

.mainNavbar_inner {
    width: 82%;
    height: 30px;
    display: flex;
    justify-content: space-between;
    align-items: center;
    border-bottom: 1px solid #D9D9D9;
}

.mainNavbar_inner h5 {
    color: black;
    font-size: 13px;
    font-weight: 400;
    margin: 0;
}

.questionWrapper {
    display: flex;
}

.question {
    background: #F0F3FA;
    border-radius: 50%;
    width: 20px;
    height: 20px;
    display: flex;
    align-items: center;
    justify-content: center;
    margin-left: 3px;
    margin-top: -10px;
}

.main_inner__tableBlock {
    margin-top: 50px;
    display: flex;
}

@media screen and (max-width: 612px) {
    .main_inner__tableBlock {
        flex-direction: column-reverse;
        align-items: center;
    }
}

.bg-left {
    position: absolute;
    width: 120px;
    top: 100px;
    left: 0px;
    z-index: -1;
}

.bg-right {
    position: absolute;
    width: 50%;
    top: 150px;
    right: 0px;
    z-index: -1;
}

.descriptionBlock_wrapper {
    text-align: left;
    width: 45%;
}

.descriptionBlock h4 {
    color: #42B1F4;
    font-size: 17px;
    font-weight: 400;
    margin: 10px 0;
}

.descriptionBlock h5 {
    color: black;
    font-size: 13px;
    font-weight: 400;
    margin: 6px 0;
}

.dots {
    margin-right: 8px;
}

.getFreeBtn {
    color: white;
    background: #43A9FE;
    border-radius: 50px;
    padding: 14px 19px;
    border: none;
    margin-top: 25px;
}

.tableBlock_wrapper {
    width: 50%;
}

.tableImg {
    max-width: 130%;
}
</style>
  