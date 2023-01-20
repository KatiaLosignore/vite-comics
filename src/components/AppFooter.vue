<script>
export default {
    name: 'AppFooter'
};

</script>

<template>
    <footer>
        <div class="container">

            <nav class="footer-nav">
                <div class="footer-col">
                    <div>
                        <h4>DC COMICS</h4>
                        <ul>
                            <li><a href="#">Characters</a></li>
                            <li><a href="#">Comics</a></li>
                            <li><a href="#">Movies</a></li>
                            <li><a href="#">TV</a></li>
                            <li><a href="#">Games</a></li>
                            <li><a href="#">Videos</a></li>
                            <li> <a href="#">News</a></li>
                        </ul>
                        <h4 class="special">SHOP</h4>
                        <ul>
                            <li><a href="#">Shop DC</a></li>
                            <li><a href="#">Shop DC Collectibles</a></li>
                        </ul>
                    </div>
                </div>
                <div class="footer-col">
                    <div>
                        <h4>DC</h4>
                        <ul>
                            <li><a href="#">Terms Of Use</a></li>
                            <li><a href="#">Privacy policy (New)</a></li>
                            <li><a href="#">Ad Choices</a></li>
                            <li><a href="#">Advertising</a></li>
                            <li><a href="#">Jobs</a></li>
                            <li><a href="#">Subscriptions</a></li>
                            <li> <a href="#">Talent Workshops</a></li>
                            <li> <a href="#">CPSC Certificates</a></li>
                            <li> <a href="#">Ratings</a></li>
                            <li> <a href="#">Shop Help</a></li>
                            <li> <a href="#">Contact Us</a></li>
                        </ul>
                    </div>
                </div>
                <div class="footer-col">
                    <div>
                        <h4>SITES</h4>
                        <ul>
                            <li><a href="#">DC</a></li>
                            <li><a href="#">MAD Magazine</a></li>
                            <li><a href="#">DC Kids</a></li>
                            <li><a href="#">DC Universe</a></li>
                            <li><a href="#">DC Power Visa</a></li>
                        </ul>
                    </div>
                </div>

                <div class="footer-col-img">
                    <img src="../assets/img/dc-logo-bg.png" alt="logo">
                </div>
    
            </nav>
        </div>

        <div class="footer-bottom">

            <div class="container">
                <nav class="footer-nav-bottom">
                    <h5>SIGN-UP NOW!</h5>
                
                    <ul>
                        <li><a href="#" class="special">FOLLOW US</a></li>
                        <li><img src="../assets/img/footer-facebook.png" alt=""></li>
                        <li><img src="../assets/img/footer-twitter.png" alt=""></li>
                        <li><img src="../assets/img/footer-youtube.png" alt=""></li>
                        <li><img src="../assets/img/footer-pinterest.png" alt=""></li>
                        <li><img src="../assets/img/footer-periscope.png" alt=""></li>
                    </ul>
                </nav>
                
            </div>

        </div>        

    </footer>


</template>

<style scoped>

    footer {                   
        padding-top: 200px;
        background-image: url('../assets/img/footer-bg.jpg');
        background-position: bottom;
        height: 960px;
    }
    
    .footer-nav {
        display: flex;
        justify-content: space-between;
        margin-bottom: 3rem;
        width: 100%;
    }

    .footer-col {
        display: flex;
        justify-content: space-between;
        padding: 0 1rem;
        width: 15%;
    }

    .footer-col-img {
        width: 50%;
    }

    .footer-col-img img{
        height: 126%;
    }

    .footer-col h4 {
        font-weight: 600;
        font-size: 1rem;
        margin-bottom: 1rem;
        color: white;
    }

    .special {
        margin-top: 15px;
    }

    .footer col ul li a.follow {
        font-size: 100px;
        font-weight: 600;
    }

    .footer-col ul {
        list-style-type: none;
    }

    .footer-col ul li a {
        display: inline-block;
        margin-bottom: 0.25rem;
        font-size: 13px;
        color: darkgrey;
    }

    .footer-bottom {
        position: relative;
        z-index: 1;
        background-color: rgb(48,48,48);
        height: 100px;
        width: 100%;
    }

    .footer-nav-bottom {
        display: flex;
        justify-content: space-between;
    }

    .footer-nav-bottom ul{
        display: flex;
        justify-content: center;
        align-items: center;
        margin: 30px;
        padding: 0;
    }

    .footer-nav-bottom ul li {
        list-style-type: none;
        font-weight: bold;
        font-size: 13px;
    }

    .footer-nav-bottom h5 {
        color: white;
        cursor: pointer;
        margin-top: 30px;
        height: 37px;
        padding: 8px;
        border: 2px solid rgb(2,130,249);
    }

    li a.special {
        color: rgb(2,130,249);
        font-size: 15px;
        margin-right: 10px;
    }

    ul li img {
        margin: 0 10px;
        cursor: pointer;
    }


</style>