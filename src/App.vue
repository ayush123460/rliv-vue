<template>
  <div id="app">
        <header>
            <div class="container">
                <!-- Left Side Navigation -->
                <div class="left">
                    <router-link to="/" exact>home</router-link>
                    <router-link to="tournaments">tournaments</router-link>
                </div>
                <!-- Logo -->
                <div class="main">
                    <img src="../public/img/logo.png" alt="RL India Logo" class="logo">
                    RL INDIA
                </div>
                <!-- Right side Navigation -->
                <div class="right">
                    <router-link to="about">about</router-link>
                    <router-link to="donate">donate</router-link>
                    <router-link to="contact">contact</router-link>
                </div>
                <div class="mob" @click="toggleMenu()" ref="mob">
                    <div class="bar"></div>
                    <div class="bar"></div>
                    <div class="bar"></div>
                </div>
                <div class="mobile" ref="mobile">
                    <router-link to="/">home</router-link>
                    <router-link to="tournaments">tournaments</router-link>
                    <router-link to="about">about</router-link>
                    <router-link to="donate">donate</router-link>
                    <router-link to="contact">contact</router-link>
                </div>
            </div>
        </header>
        <router-view />
        <footer>
            &copy; 2019 RL India All Rights Reserved. &copy; 2019 Psyonix, Inc. All Rights to Rocket League Reserved.
        </footer>
    </div>
</template>

<script>
export default {
    methods: {
        toggleMenu: function() {
            // function to toggle the menu in Mobile viewport.
            let m = this.$refs.mob;
            let mb = this.$refs.mobile;
            m.classList.toggle('active');
            mb.classList.toggle('active');
            document.getElementsByTagName("body")[0].classList.toggle('overflow');
        }
    }
}
</script>


<style lang="scss">
@import './sass/main';
</style>
