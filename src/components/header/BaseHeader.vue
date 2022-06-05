<template>
    <header>
        <div class="container">
            <div class="header__logo">
                <img src="../../assets/img/dc-logo.png" alt="DC-Logo">
            </div>
            <nav class="header__nav">
                <ul>
                    <li v-for="(link, index) in links" :key="index">
                        <a :class="{active : link.current}" :href="link.url">{{link.text}}</a>
                    </li>
                </ul>
            </nav>
        </div>
    </header>
</template>

<script>
export default {
    name: 'BaseHeader',
    data() {
        return {
            links: [
                {
                    text: "characters",
                    url: "#",
                    current: false,
                },
                {
                    text: "comics",
                    url: "#",
                    current: true,
                },
                {
                    text: "movies",
                    url: "#",
                    current: false,
                },
                {
                    text: "tv",
                    url: "#",
                    current: false,
                },
                {
                    text: "games",
                    url: "#",
                    current: false,
                },
                {
                    text: "collectibles",
                    url: "#",
                    current: false,
                },
                {
                    text: "videos",
                    url: "#",
                    current: false,
                },
                {
                    text: "fans",
                    url: "#",
                    current: false,
                },
                {
                    text: "news",
                    url: "#",
                    current: false,
                },
                {
                    text: "shop",
                    url: "#",
                    current: false,
                },
            ]
        }
    }
}
</script>

<style lang='scss' scoped>
@import '../../assets/style/mixins.scss';

header {
    background-color: var(--primay-color);

    .container {
        @include flexCenter;
    }

    nav ul li{
        @include sterileLi;
    }

    nav ul li a {
        text-decoration: none;
        color: black;
        text-transform: uppercase;
        font-weight: 700;
    }

    a.active {
        border-bottom: .500rem solid var(--secondary-color);
        color: var(--secondary-color);
    }
}
</style>