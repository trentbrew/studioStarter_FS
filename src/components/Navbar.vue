<template>
<div id="nav">
    <ul>
        <router-link to="/"><li class="nav-item">Home</li></router-link>
        <router-link to="/library"><li class="nav-item">Library</li></router-link>
    </ul>
</div>
</template>

<script>
export default {
    name: 'Navbar',
    data() {
        return {

        }
    },
    created() {

    },
    mounted() {

    },


}
</script>

<style lang="scss" scoped>
@import '../assets/styles/_global';

#nav {
    background: $colorMain;
    box-shadow: $shadow;
    height: $navHeight;
    width: 100%;
    justify-content: center;
    align-items: center;
    line-height: $navHeight;
    text-align: center;

    ul {
        text-decoration: none;
        list-style: none;
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 0px;
        padding: 0px;

        li.nav-item {
            cursor: pointer;
            font-weight: normal;
            padding-left: $nudge;
            padding-right: $nudge;
            height: $navHeight;
            transition: $quick;

            &:hover {
                background: $colorLightGray;
            }
        }
    }

    a {
        height: $navHeight;
        text-decoration: none;
        color: black;

    }

    a.router-link-exact-active {
        font-weight: bold;
    }
}

</style>