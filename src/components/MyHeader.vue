<template>
    <div id="header">
        <!-- logo a sx -->
        <div>
            <img src="../assets/dc-logo.png" alt="">
        </div>

        <!-- nav a dx -->
        <nav>
            <a href="" v-for="(navTags,i) in nav" :key="i">{{navTags.navTag}}</a>
            <!-- <a href="">COMICS</a>
            <a href="">MOVIES</a>
            <a href="">TV</a>
            <a href="">GAMES</a>
            <a href="">COLLECTIBLES</a>
            <a href="">VIDEOS</a>
            <a href="">FANS</a>
            <a href="">NEWS</a>
            <a href="">SHOP</a> -->
        </nav>
        <!-- <h1>Header</h1> -->
    </div>
</template>

<script>
export default {
    name: 'MyHeader',
    data() {
        return {
            nav: [
                {
                    navTag: 'CHARACTERS'
                },
                {
                    navTag: 'COMICS'
                },
                {
                    navTag: 'MOVIES'
                },
                {
                    navTag: 'TV'
                },
                {
                    navTag: 'GAMES'
                },
                {
                    navTag: 'COLLECTABLES'
                },
                {
                    navTag: 'VIDEOS'
                },
                {
                    navTag: 'FANS'
                },
                {
                    navTag: 'NEWS'
                },
                {
                    navTag: 'SHOP'
                },
            ]
        }
    }
}
</script>

<style scoped lang="scss">
#header {
    display: flex;
    flex-direction: row;
    justify-content: space-between;
    align-items: center;
    padding-top: 10px;
    padding-bottom: 10px;
    padding-left: 10%;
    padding-right: 10%;

    a {
        text-decoration: none;
        color: #303030;
        margin-right: 10px;

        &:hover {
            color: #0282f9;
        }
    }
}
</style>
