<template>
    <footer>
        <div class="background">
            <div class="container">

        </div>
        </div>
        <div class="last_section">
            <div class="container">
                <button>
                   Sign-up&minus;now&excl;
                </button>
                <ul>
                    <li>
                        <a href="#">FOLLOW US</a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-facebook-f"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-twitter"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-youtube"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fab fa-pinterest"></i>
                        </a>
                    </li>
                    <li>
                        <a href="#">
                            <i class="fas fa-map-marker-alt"></i>
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
        line-height: 100px;
    }
    li {
        list-style: none;
    }
    li a {
        margin: 0 15px;
        text-decoration: none;
        color: #2179E5;
    }
    a i {
        height: 30px;
        width: 30px;
        padding: 10px;
        color: #303030;
        background-color: #797979;
        border-radius : 50px;
    }
</style>