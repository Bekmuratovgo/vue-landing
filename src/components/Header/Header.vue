<template>
    <div class="header">
        <div class="header_inner">
            <div class="logo">
                <img src="../../assets/img/logo.png" alt="">
            </div>
            <div class="navbar">
                <div class="nav">
                    <h5>Цены</h5>
                </div>
                <div class="nav">
                    <h5>Отзывы</h5>
                </div>
                <div class="nav">
                    <h5>Особенности платформы</h5>
                </div>
                <div class="nav"><button>Авторизоваться</button></div>
                <div class="nav">
                    <div class="nav_imgProfile">
                        <img src="../../assets/img/profile.png" alt="">
                    </div>
                    <h5>EN</h5>
                </div>
            </div>
            <div class="menuBurger">
                <img src="../../assets/img/menu.png" alt="">
            </div>
        </div>
    </div>
</template>
  
<script>

export default {
    name: 'Header-Component',
    components: {
    }
}
</script>
  
<style>
.header {
    background: #FFFFFF;
    box-shadow: 0px 4px 15px rgba(0, 0, 0, 0.05);
    width: 100%;
    height: 98px;
    display: flex;
    justify-content: center;
}
.header_inner {
    height: 100%;
    display: flex;
    align-items: center;
    justify-content: space-between;
    width: 80%;
}
.logo {
    width: 35%;
    text-align: left;
}

.navbar {
    width: 70%;
    display: flex;
    justify-content: space-between;
}

.nav {
    display: flex;
    align-items: center;
}

.nav_imgProfile {
    background: #f4d170;
    border-radius: 50%;
    width: 30px;
    height: 30px;
    display: flex;
    align-items: center;
    justify-content: center;
}

.nav_imgProfile img {
    width: 14px;
    height: 14px;
}

.nav button {
    background: #43a9fe;
    color: white;
    border: none;
    border-radius: 50px;
    padding: 12px 19px;
    font-weight: 400;
    font-size: 13px;
    display: flex;
    align-items: center;
}

.nav h5 {
    margin-top: 0;
    margin-bottom: 0;
    font-size: 15px;
    font-weight: 400;
}
.menuBurger {
    display: none;
}
@media screen and (max-width: 940px) {
    .navbar {
        display: none !important;
    }
    .menuBurger {
        display: block;
    }
    .menuBurger img {
        width: 50px;
    }
}
</style>
  