<template>
    <header>
        <a href="#"> 
            <img src="../assets/dc-logo.png" alt="DC logo">
        </a> 
            <nav>
                <ul>
                    <li>
                        <a href="#">characters</a>
                    </li>
                    <li>
                        <a href="#" class="active">comics</a>
                    </li>
                    <li>
                        <a href="#">movies</a>
                    </li>
                    <li>
                        <a href="#">tv</a>
                    </li>
                    <li>
                        <a href="#">games</a>
                    </li>
                    <li>
                        <a href="#">collectibles</a>
                    </li>
                    <li>
                        <a href="#">videos</a>
                    </li>
                    <li>
                        <a href="#">fans</a>
                    </li>
                    <li>
                        <a href="#">news</a>
                    </li>
                    <li>
                        <a href="#">shop</a>
                    </li>    
                </ul>
            </nav>
    </header>
</template>

<script>
export default {
    name : "Header",
}
</script>

<style scoped>
    header {
        display: flex;
        justify-content: space-between;
        height: 120px;
        max-width: 70%;
        margin : auto;
    }
    header > a {
        display: flex;
    }
    img {
        height: 80%;
        align-self: center;
    }
    ul {
        display: flex;
    }
    ul > li {
        list-style: none;
    }
    li > a {
        line-height: 120px;
        text-decoration: none;
        text-transform: uppercase;
        padding: 0 10px;
        color: #4F4948;
    }
    .active,
    li > a:hover  {
        padding-bottom: 46px;
        color: #2179E5;
        border-bottom: 5px solid #2179E5;
    }
</style>