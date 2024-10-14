<template>
    <div class="admin-layout">
        <Header />
        <div class="content">
            <Menu />
            <Main />
        </div>
        <Footer />
    </div>
</template>

<script setup>
import Header from './Header.vue';
import Menu from './Menu.vue';
import Main from './Main.vue';
import Footer from './Footer.vue';
</script>

<style scoped>
.admin-layout {
    display: flex;
    flex-direction: column;
    height: 100vh;
}

.content {
    display: flex;
    flex: 1;
}

header {
    height: 50px;
    background-color: #d3dce6;
}

menu {
    width: 200px;
    background-color: #1e3a8a;
    color: white;
}

main {
    flex: 1;
    background-color: #f8fafc;
}

footer {
    height: 50px;
    background-color: #d3dce6;
}
</style>