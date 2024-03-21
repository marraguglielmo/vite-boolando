<script>
    export default{}
</script>

<template>
    <header>
        <section class="container d-flex ">
            <!-- TOPBAR -->
            <nav>
                <ul class="categories d-flex ">
                    <li><a href="#">Donna</a></li>
                    <li><a href="#">Uomo</a></li>
                    <li><a href="#">Bambini</a></li>
                </ul>
            </nav>
            <!-- /TOPBAR -->
            <!-- LOGO -->
            <span class="logo ">
                <!-- <p>logo</p> -->
                <img src="../../boolean-logo.png" alt="logo">
            </span>
            <!-- /LOGO -->
            <!-- MENU -->
            <span>
                <nav>
                    <ul class="menu d-flex">
                        <li><a href="#"><i class="fa-regular fa-user"></i></a></li>
                        <li><a href="#"><i class="fa-regular fa-heart"></i></a></li>
                        <li><a href="#"><i class="fa-solid fa-bag-shopping"></i></a></li>
                    </ul>
                </nav>
            </span>
            <!-- /MENU -->
        </section>
    </header>
</template>

<style lang="scss" scoped>
@use '../assets/scss/partials/variables' as *;

header{
    background-color: $bg-header;
    color: white;
    position: fixed;
    width: 100%;
    top: 0;
    left: 0;
    z-index: 2;
}
</style>
