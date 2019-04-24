<template>
  <div id="app">
        <header>
        <div class="container">
            <!-- Left Side Navigation -->
            <div class="left">
                <a href="/">home</a>
                <a href="#">blog</a>
                <a href="#">tournaments</a>
            </div>
            <!-- Logo -->
            <div class="main">
                <img src="../public/img/logo.png" alt="RL India Logo" class="logo">
                RL INDIA
            </div>
            <!-- Right side Navigation -->
            <div class="right">
                <a href="#">about</a>
                <a href="#">donate</a>
                <a href="#">contact</a>
            </div>
            <div class="mob" onclick="toggleMenu()">
                <div class="bar"></div>
                <div class="bar"></div>
                <div class="bar"></div>
            </div>
            <div class="mobile">
                <a href="/">home</a>
                <a href="#">tournaments</a>
                <a href="#">about</a>
                <a href="#">donate</a>
                <a href="#">contact</a> --}}
                <button class="btn btn-primary">Login</button>
            </div>
        </div>
    </header>
    <router-view />
    <footer>
        &copy; 2019 RL India All Rights Reserved. &copy; 2019 Psyonix, Inc. All Rights to Rocket League Reserved.
    </footer>
  </div>
</template>

<style lang="scss">
@import './sass/main';
</style>
