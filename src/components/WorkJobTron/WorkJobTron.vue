<template>
    <div class="workJob">
        <h2 class="workJob_title">
            <img class="titleImg" src="../../assets/img/titleImg.png" />С JOBTRON работать легко и удобно
        </h2>
        <p class="workJob_desc">Мы заботимся о наших клиентах и предоставляем индивидуальный подход, который будет полезен каждому</p>
        
        <div class="workJob_inner">
            <div class="block-left">
                <img src="../../assets/img/table.png">
            </div>
            <div class="block-right">
                <h4>Интеграция с вашей  CRM-системой</h4>
                <p>Корпоративный портал JOBTRON может интегрироваться с разными CRM, сревисами рассылки, системами учета времени и трекинга, в также с другими многофункциональными сервисами</p>
            </div>
        </div>
        
        <div class="workJob_inner_second">
            <div class="block-right">
                <h4>Служба поддержки</h4>
                <p>Корпоративный портал JOBTRON может интегрироваться с разными CRM, сревисами рассылки, системами учета времени и трекинга, в также с другими многофункциональными сервисами</p>
            </div>
            <div class="block-left">
                <img src="../../assets/img/table.png">
            </div>
        </div>

        <div class="workJob_inner_third">
            <div class="block-left">
                <img src="../../assets/img/table.png">
            </div>
            <div class="block-right">
                <h4>Гибкие возможности</h4>
                <p>Корпоративный портал JOBTRON может интегрироваться с разными CRM, сревисами рассылки, системами учета времени и трекинга, в также с другими многофункциональными сервисами</p>
            </div>
        </div>

    </div>
</template>
  
<script>
export default {
    name: 'WorkJob-Component',
    components: {
    }
}
</script>
  
<style>
.workJob {
    margin-top: 160px;
}
.workJob_title {
    display: flex;
    align-items: center;
    justify-content: center;
    margin: 0;
}
.workJob_desc {
    display: flex;
    justify-content: center;
    font-size: 15px;
}
.workJob_inner {
    margin-top: 50px;
    display: flex;
    text-align: left;
    background-image: url(../../assets/img/job-right.png);
    background-size: contain;
    background-repeat: no-repeat;
    background-position-x: right;
}
.workJob_inner_second {
    margin-top: 50px;
    display: flex;
    text-align: left;
    background-image: url(../../assets/img/job-left.png);
    background-size: contain;
    background-repeat: no-repeat;
    background-position-x: left;
}
.workJob_inner_third {
    margin-top: 50px;
    display: flex;
    text-align: left;
    background-image: url(../../assets/img/job-left-2.png);
    background-size: contain;
    background-repeat: no-repeat;
    background-position-x: left;
}

.block-left {
    width: 50%;
}
.block-right {
    width: 50%;
    padding: 0 20px;
}
.block-left img {
    width: 100%;
}
</style>
  