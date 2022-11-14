<template>
    <div class="footer">
        <div class="footer_inner">
            <div>
                <img src="../../assets/img/logo-white.png" alt="">
            </div>
            <div>
                <h5>Цены</h5>
                <h5>Отзывы</h5>
                <h5>Особенности платформы</h5>
                <div class="footer_inner__details">
                    <h5>Подпишитесь на новости:</h5>
                    <div class="footer_inner__icons">
                        <img src="../../assets/img/telegram.png" alt="">
                        <img src="../../assets/img/instagram.png" alt="">
                        <img src="../../assets/img/youtube.png" alt="">
                    </div>
                </div>
            </div>
            <div>
                <h5>Документы</h5>
                <h5>Информация об оплате</h5>
                <h5>Лицензионное соглашение</h5>
                <div class="footer_inner__details">
                    <h5>Способы оплаты:</h5>
                    <div class="footer_inner__icons">
                        <img src="../../assets/img/mir.png" alt="">
                        <img src="../../assets/img/visa.png" alt="">
                        <img src="../../assets/img/iomoney.png" alt="">
                    </div>
                </div>
            </div>
            <div>
                <h5>Отдел продаж</h5>
                <h5>8 777 788 08 00</h5>
                <h5>8 777 788 08 00</h5>
                <h5>sales@jobtron.com</h5>
                <div style="margin-top: 10px">
                    <h5>Отдел продаж:</h5>
                    <h5>support@jobtron.com</h5>
                </div>
            </div>
        </div>
        <div class="footer_under">
            <div class="footer_under__inner">
                <h5>© 2022 «Jobton», Все права защищены</h5>
                <div class="footer_under__inner_block">
                    <h5>Правила сайта</h5>
                    <h5>Политика конфиденциальности</h5>
                </div>
            </div>
        </div>
    </div>
</template>
  
<script>

export default {
    name: 'Footer-Component',
    components: {
    }
}
</script>
  
<style>
.footer {
    background: #424d53;
    width: 100%;
    display: flex;
    flex-direction: column;
    align-items: center;
}

.footer h5 {
    color: white;
    font-size: 13px;
    font-weight: 400;
    margin: 8px 0
}

.footer_inner {
    width: 80%;
    margin-top: 53px;
    display: flex;
    justify-content: space-between;
    text-align: left;
    flex-wrap: wrap;
}
.footer_inner__icons {
    display: flex;
    align-items: center;
}
.footer_inner__icons img {
    margin-right: 12px;
}
.footer_inner__details {
    margin-top: 36px;
}
.footer_under {
    display: flex;
    width: 100%;
    height: 72px;
    justify-content: center;
    border-top: 1px solid #72C6F9;
}

.footer_under__inner {
    width: 80%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}
.footer_under__inner_block {
    display: flex;
}
.footer_under__inner_block h5 {
    margin: 0 10px;
}
</style>
  