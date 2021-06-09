<template>
    <footer>
        <div class="background">
            <div class="container">
                <div class="vertical_list">
                    <ul>
                        <li>
                            <a href="#">
                                <h3>dc comics</h3>
                            </a>
                        </li>
                        <li v-for="(item,index) in comics" :key="index">
                            <a :href="item.link">{{item.text}}</a>
                        </li>
                    </ul>
                    <ul class="vertical_list">
                        <li>
                            <a href="">
                                <h3>shop</h3>
                            </a>
                        </li>
                       <li v-for="(item,index) in shop" :key="index">
                            <a :href="item.link">{{item.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="vertical_list">
                    <ul>
                        <li>
                            <a href=""><h3>dc</h3></a>
                        </li>
                        <li v-for="(item,index) in dc" :key="index">
                            <a :href="item.link">{{item.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="vertical_list">
                    <ul>
                        <li>
                            <a href="#"><h3>sites</h3></a>
                        </li>
                        <li v-for="(item,index) in sites" :key="index">
                            <a :href="item.link">{{item.text}}</a>
                        </li>
                    </ul>
                </div>
                <div class="backg_logo"></div>
            </div>
        </div>
        <div class="last_section">
            <div class="container">
                <button>
                   Sign-up&minus;now&excl;
                </button>
                <ul>
                    <li>
                        <a href="#"><span>FOLLOW US </span></a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/footer-facebook.png" alt="logo_facebook">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/footer-twitter.png" alt="logo_twitter">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/footer-youtube.png" alt="logo_youtube">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/footer-pinterest.png" alt="logo_pinterest">
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <img src="../assets/footer-periscope.png" alt="logo_periscope">
                        </a>
                    </li>
                </ul>
            </div>
        </div>
    </footer>
    
</template>

<script>
export default {
    name : "Footer",
    data: function () {
        return {
            comics : [
                {
                    text:"Charachters",
                    link:"#Charachters"
                },
                {
                    text:"Comics",
                    link:"#Comics"
                },
                {
                    text:"Movies",
                    link:"#Movies"
                },
                {
                    text:"TV",
                    link:"#TV"
                },
                {
                    text:"Games",
                    link:"#Games"
                },
                {
                    text:"Videos",
                    link:"#Videos"
                },
                {
                    text:"News",
                    link:"#News"
                },
            ],
            shop: [
                {
                    text: "Shop DC",
                    link: "#Shop_DC"
                },
                {
                    text: "Shop Dc Collectibles",
                    link: "#Shop_Dc_Collectibles"
                }
            ],
            dc: [
                {
                    text: "Terms Of Use",
                    link: "#Terms_Of_Use"
                },
                {
                    text: "Privacy Policy (New)",
                    link: "#Privacy_policy"
                },
                {
                    text: "Ad Choices",
                    link: "#ad_choices"
                },
                {
                    text: "Advertising",
                    link: "#advertising"
                },
                {
                    text: "Jobs",
                    link: "#jobs"
                },
                {
                    text: "Subscriptions",
                    link: "#subscriptions"
                },
                {
                    text: "Talent Workshops",
                    link: "#talent_workshops"
                },
                {
                    text: "CPSC Certificates",
                    link: "#CPSC_certificates"
                },
                {
                    text: "Ratings",
                    link: "#ratings"
                },
                {
                    text: "Shop Help",
                    link: "#shop_help"
                },
                {
                    text: "Contact Us",
                    link: "#contact_us"
                },
            ],
            sites: [
                {
                    text: "DC",
                    link: "#dc"
                },
                {
                    text: "MAD Magazine",
                    link: "#mad_magazine"
                },
                {
                    text: "DC Kids",
                    link: "#dc_kids"
                },
                {
                    text: "DC Universe",
                    link: "#dc_universe"
                },
                {
                    text: "DC Power Visa",
                    link: "#dc_power_visa"
                },
            ]
        }
    }
}
</script>

<style lang="scss" scoped>
    .background {
        background-image: url("../assets/footer-bg.jpg");
        background-repeat: repeat-x;
        height: 350px;
    }
    .backg_logo {
        background-image: url("../assets/dc-logo-bg.png");
        height: 350px;
        Width: 100%;
        background-repeat: no-repeat;
        background-position: right;
    }
    .container {
        display: flex;
        max-width: 70%;
        margin: auto;
    }
    .last_section {
        height: 100px;
        background-color: #303030;
            & .container {
                display: flex;
                justify-content: space-between;
            }
    }
    button {
        align-self: center;
        padding: 10px;
        text-transform: uppercase;
        font-size: 14px;
        font-weight: 700;
        cursor: pointer;
        background-color: #303030;
        border: 2px solid #2179E5;
        color: white;
            &:hover{
                background-color: #2179E5;
            }
    }
    ul {
        display: flex;
    }
    .last_section li {
        list-style: none;
        line-height: 97px;
        align-self: center;
            span {
                 margin-right: 20px;
                font-size: 18px;
                font-weight: 700;
                color: #2179E5;
            }
            a {
                text-decoration: none;
            }
            img {
                height: 40px;
                vertical-align: middle;
                padding: 0 7px;
            } &:hover {
                opacity: 0.8;
            }
    }
    .vertical_list {
        display: flex;
        flex-direction: column;
        margin-top: 20px;
        justify-content: flex-start;
            ul {
                flex-direction: column;
                width: 140px;
            }
            li {
                list-style: none;
                font-weight: bold;
                font-size: 12px;
                padding: 2px;
            }
            a {
                text-decoration: none;
                color: #797979;
            }
            a:hover {
                color:#2179E5;
            }
            h3 {
                font-size: 18px;
                margin-bottom: 10px;
                text-transform: uppercase;
                color: white;
            }
    }
</style>