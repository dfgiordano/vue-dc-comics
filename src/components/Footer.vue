<template>
    <footer>
        <div class="background">
            <div class="container">
                <div class="vertical_list">
                    <ul>
                        <li><h3>dc comics</h3></li>
                        <li>Charachters</li>
                        <li>Comics</li>
                        <li>Movies</li>
                        <li>Games</li>
                        <li>Videos</li>
                        <li>News</li>
                    </ul>
                    <ul class="vertical_list">
                        <li><h3>shop</h3></li>
                        <li>Shop DC</li>
                        <li>Shop Dc Collectibles</li>
                    </ul>
                </div>
                <div class="vertical_list">
                    <ul>
                        <li><h3>dc</h3></li>
                        <li>Terms Of Use</li>
                        <li>Privacy Policy (New)</li>
                        <li>Ad Choices</li>
                        <li>Advertising</li>
                        <li>Jobs</li>
                        <li>Subscriptions</li>
                        <li>Talent Workshops</li>
                        <li>CPSC Certificates</li>
                        <li>Ratings</li>
                        <li>Shop Help</li>
                        <li>Contact Us</li>
                    </ul>
                </div>
                <div class="vertical_list">
                    <ul>
                        <li><h3>sites</h3></li>
                        <li>DC</li>
                        <li>MAD Magazine</li>
                        <li>DC Kids</li>
                        <li>DC Universe</li>
                        <li>DC Power Visa</li>
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
}
</script>

<style scoped>
    .background {
        background-image: url("../assets/footer-bg.jpg");
        background-repeat: repeat-x;
        height: calc(100vh - 490px);
        /* height: 400px; */
    }
    .backg_logo {
        background-image: url("../assets/dc-logo-bg.png");
        height: 479px;
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
    }
    .last_section .container {
        display: flex;
        justify-content: space-between;
    }
    button {
        align-self: center;
        padding: 10px;
        text-transform: uppercase;
        font-size: 14px;
        font-weight: 700;
        cursor:pointer;
        background-color: #303030;
        border: 2px solid #2179E5;
        color: white;
    }
    ul {
        display: flex;
    }
    .last_section li {
        list-style: none;
        line-height: 97px;
        align-self: center;
    }
    .last_section li span {
        margin-right: 20px;
        font-size: 18px;
        font-weight: 700;
        color: #2179E5;
    }
    .last_section li a {
        text-decoration: none;
    }
    .last_section li img {
        height: 30px;
        vertical-align: middle;
        padding: 0 7px;
    }
    .vertical_list {
        display: flex;
        flex-direction: column;
        margin-top: 30px;
        justify-content: flex-start;
    }
    .vertical_list > ul {
        flex-direction: column;
        width: 140px;
    }
    .vertical_list li {
        list-style: none;
        font-size: 12px;
        padding: 2px;
        color: #797979;
    }
    .vertical_list h3 {
        font-size: 18px;
        margin-bottom: 20px;
        text-transform: uppercase;
        color: white;
    }
</style>