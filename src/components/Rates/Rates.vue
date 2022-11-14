<template>
    <div class="rates">
        <h2 class="workJob_title">
            <img class="titleImg" src="../../assets/img/titleImg.png" />Тарифы
        </h2>
        <div class="rates_inner">
            <table class="table">
                <thead class="thead">
                    <tr>
                        <th class="firstTh" scope="col"></th>
                        <th class="secondTh" scope="col">Бесплатный</th>
                        <th class="thirdTh" scope="col">База</th>
                        <th class="fourthTh" scope="col">Стандарт</th>
                        <th class="fifthTh" scope="col">PRO</th>
                    </tr>
                </thead>
                <tbody>
                    <tr>
                        <th scope="row">Количество пользователей</th>
                        <td>до 5</td>
                        <td>до 20</td>
                        <td>до 50</td>
                        <td>до 100</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Место</th>
                        <td class="trBgBlue">5 Гб</td>
                        <td class="trBgBlue">20 Гб</td>
                        <td class="trBgBlue">50 Гб</td>
                        <td class="trBgBlue">1 T</td>
                    </tr>
                    <tr>
                        <th scope="row">База знаний</th>
                        <td>+</td>
                        <td>+</td>
                        <td >+</td>
                        <td >+</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Новости</th>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                    </tr>
                    <tr>
                        <th scope="row">Обучение</th>
                        <td>+</td>
                        <td>+</td>
                        <td >+</td>
                        <td >+</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Аналитика</th>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                    </tr>
                    <tr>
                        <th scope="row">Контроль качества</th>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Чат</th>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                    </tr>
                    <tr>
                        <th scope="row">Структура компании</th>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Поддержка</th>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                    </tr>
                    <tr>
                        <th scope="row">Администрирование/аудит</th>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Перенос на сервер клиента</th>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                    </tr>
                    <tr>
                        <th scope="row">Индивидуальный домен клиента</th>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                        <td >+</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Брендирование кабинета (размещение логотипа, фирменный цвет</th>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                        <td class="trBgBlue">+</td>
                    </tr>
                    <tr>
                        <th scope="row">Оплата в месяц</th>
                        <td ></td>
                        <td >9 000</td>
                        <td >27 000</td>
                        <td >100 000</td>
                    </tr>
                    <tr>
                        <th class="trBgBlue" scope="row">Оплата в год</th>
                        <td class="trBgBlue"></td>
                        <td class="trBgBlue">108 000</td>
                        <td class="trBgBlue">291 600</td>
                        <td class="trBgBlue">960 000</td>
                    </tr>
                    <tr>
                        <th scope="row">Скидка</th>
                        <td ></td>
                        <td ></td>
                        <td >20%</td>
                        <td >20%</td>
                    </tr>
                </tbody>
            </table>
        </div>
    </div>
</template>
  
<script>
export default {
    name: 'Rates-Component',
    components: {
    },
    data() {
        return {
            items: [
                { age: 40, first_name: 'Dickerson', last_name: 'Macdonald' },
                { age: 21, first_name: 'Larsen', last_name: 'Shaw' },
                { age: 89, first_name: 'Geneva', last_name: 'Wilson' },
                { age: 38, first_name: 'Jami', last_name: 'Carney' }
            ]
        }
    },
}
</script>
  
<style>
.rates {
    margin-top: 150px;
}
.rates_inner {
    margin-top: 20px;
}
.rates h2 {
    font-weight: 600;
    font-size: 25px;
}
.firstTh{
    width: 28%;
}
.table {
    width: 100%;
}
.thead tr {
    background: #edf8ff;
}

tr, th, td {
    border-style: none !important;
}
.trBgWhite {
    background: white !important;
}
.trBgBlue {
    background: #edf8ff !important;
}


</style>
  