<template>
    <footer>
        <div class="background">
            <div class="container">
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
    }
    .backg_logo {
        background-image: url("../assets/dc-logo-bg.png");
        height: 300px;
        WIDTH: 100%;
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
        padding: 15px;
        text-transform: uppercase;
        font-size: 18px;
        cursor:pointer;
        background-color: #303030;
        border: 2px solid #2179E5;
        color: white;
    }
    ul {
        display: flex;
        align-self: center;
    }
    li {
        list-style: none;
        line-height: 97px;
        align-self: center;
    }
    li span {
        margin-right: 20px;
        font-size: 20px;
        font-weight: bold;
        color: #2179E5;
    }
    li a {
        text-decoration: none;
    }
    li img {
        height: 30px;
        vertical-align: middle;
        padding: 0 7px;
    }
</style>