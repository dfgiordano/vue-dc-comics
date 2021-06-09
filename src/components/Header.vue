<template>
    <header>
        <a href="#"> 
            <img src="../assets/dc-logo.png" alt="DC logo">
        </a> 
            <nav>
                <ul>
                    <li v-for="(item,index) in menu" :key="index">
                        <a :href="item.link">{{item.text}}</a>
                    </li>
                </ul>
            </nav>
    </header>
</template>

<script>
export default {
    name : "Header",
    data: function () {
        return {
            menu: [
                {
                    text: "characters",
                    link: "#characters",
                    active: false,
                },
                {
                    text: "comics",
                    link: "#comics",
                    active: true,
                },
                {
                    text: "movies",
                    link: "#movies",
                    active: false,
                },
                {
                    text: "tv",
                    link: "#tv",
                    active: false,
                },
                {
                    text: "games",
                    link: "#games",
                    active: false,
                },
                {
                    text: "collectibles",
                    link: "#collectibles",
                    active: false,
                },
                {
                    text: "videos",
                    link: "#videos",
                    active: false,
                },
                {
                    text: "fans",
                    link: "#fans",
                    active: false,
                },
                {
                    text: "news",
                    link: "#news",
                    active: false,
                },
                {
                    text: "shop",
                    link: "#shop",
                    active: false,
                }

            ]
        }
    }
}
</script>

<style lang="scss" scoped>
@import "../style/variables";
    header {
        display: flex;
        justify-content: space-between;
        height: 120px;
        max-width: 70%;
        margin : auto;
            & a {
                display: flex;
            }
    }
    img {
        height: 80%;
        align-self: center;
    }
    ul {
        display: flex;
            li {
                list-style: none;
            }
                a {
                    line-height: 115px;
                    text-decoration: none;
                    text-transform: uppercase;
                    font-weight: bold;
                    padding: 0 10px;
                    color: #4F4948;
                }
    }
    .active,
    li > a:hover  {
        color: $mainColor;
        border-bottom: 5px solid $mainColor;
    }
</style>