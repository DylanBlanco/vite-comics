<script>
//import compomenenti
import appMain from './components/AppMain.vue';

export default {
    data() {
        return {
            linksMenu: [
                {
                label: 'CHARACTERS',
                url: '#',
                active: false,
                },
                {
                label: 'COMICS',
                url: '#',
                active: false,
                },
                {
                label: 'MOVIES',
                url: '#',
                active: false,
                },
                {
                label: 'TV',
                url: '#',
                active: false,
                },
                {
                label: 'GAMES',
                url: '#',
                active: false,
                },
                {
                label: 'COLLECTIBLES',
                url: '#',
                active: false,
                },
                {
                label: 'VIDEOS',
                url: '#',
                active: false,
                },
                {
                label: 'FANS',
                url: '#',
                active: false,
                },
                {
                label: 'NEWS',
                url: '#',
                active: false,
                },
                {
                label: 'SHOP',
                url: '#',
                active: false,
                },
            ],

            // footer links
            linksFooterNav:[
                {
                image: '../img/buy-comics-digital-comics.png',
                title: 'DIGITAL COMICS',
                },
                {
                image: '../img/buy-comics-merchandise.png',
                title: 'DC MERCHANDISE',
                },
                {
                image: '../img/buy-comics-subscriptions.png',
                title: 'SUBSCRICTION',
                },
                {
                image: '../img/buy-comics-shop-locator.png',
                title: 'COMIC SHOP LOCATOR',
                },
                {
                image: '../img/buy-dc-power-visa.png',
                title: 'DC POWER VISA',
                },
            ],

            // links footer links
            // linksFooterLinks: [
            //     {
            //         title: 'DC COMICS',
            //         link: [
            //             {
            //                 titleLink: 'Charater',
            //             },
            //             {
            //                 titleLink: 'Comics',
            //             },
            //             {
            //                 titleLink: 'Movies',
            //             },
            //             {
            //                 titleLink: 'TV',
            //             },
            //             {
            //                 titleLink: 'Games',
            //             },
            //             {
            //                 titleLink: 'Videos',
            //             },
            //             {
            //                 titleLink: 'News',
            //             },
            //         ]
            //     },
            //     {
            //         title: 'DC',
            //         link: [
            //             {
            //                 titleLink: 'Terms Of Use',
            //             },
            //             {
            //                 titleLink: 'Privacy Policy (New)',
            //             },
            //             {
            //                 titleLink: 'Ad Choices',
            //             },
            //             {
            //                 titleLink: 'Advertising',
            //             },
            //             {
            //                 titleLink: 'Jobs',
            //             },
            //             {
            //                 titleLink: 'Subscrictions',
            //             },
            //             {
            //                 titleLink: 'Talent Workshop',
            //             },
            //             {
            //                 titleLink: 'CPSC Certificates',
            //             },
            //             {
            //                 titleLink: 'Ratings',
            //             },
            //             {
            //                 titleLink: 'Shop Help',
            //             },
            //             {
            //                 titleLink: 'Contact us',
            //             },
            //         ]
            //     },
            //     {
            //         title: 'SITES',
            //         link: [
            //             {
            //                 titleLink: 'DC',
            //             },
            //             {
            //                 titleLink: 'MAD Magazines',
            //             },
            //             {
            //                 titleLink: 'DC Kings',
            //             },
            //             {
            //                 titleLink: 'DC Universe',
            //             },
            //             {
            //                 titleLink: 'DC Universe',
            //             },
            //             {
            //                 titleLink: 'DC Power Visa',
            //             },
            //         ]
            //     },
            //     {
            //         title: 'SHOP',
            //         link: [
            //             {
            //                 titleLink: 'Shop DC',
            //             },
            //             {
            //                 titleLink: 'Shop DC Collectibles',
            //             },
            //         ]
            //     },
            // ]
        }
    },
    components: {
        appMain
    }
}
</script>

<template>
    <!-- header -->
    <header class="container header-container">
        <div class="box-container">
            <div class="box-header-img">
                <img src="../img/dc-logo.png" alt="dc-logo">
            </div>
            <div class="box-links-header">
                <ul>
                    <li v-for="(link, i) in linksMenu" :key="i">
                        <a href="#">{{ link.label }}</a>
                    </li>
                </ul>
            </div>
        </div>
    </header>

    <!-- main -->
    <main class="container main-container">
        <appMain/>
    </main>
  
    <!-- footer -->
    <footer class="container">
        <div class="box-container">

            <!-- first section -->
            <section class="footer-nav">
                <div class="box-footer-nav">
                    <ul>
                        <li v-for="(link,i) in linksFooterNav" :key="i">
                            <a :href="link.title">
                              <img :src="link.image" :alt="link.title">
                              <p>{{ link.title }}</p>
                            </a>
                        </li>
                    </ul>
                </div>
            </section>

            <!-- second section -->
            <section class="footer-links">
                <div class="box-footer-links">
                    <div>
                        <ul>
                            <li>
                                <h4>DC COMICS</h4>
                            </li>
                            <li>
                                <a href="#">
                                    Charater
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Comics
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Movies
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    TV
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Games
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Videos
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    News
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li>
                                <h4>DC</h4>
                            </li>
                            <li>
                                <a href="#">
                                    Term Of Use
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Privacy Policy (New)
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Ad Choice
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Advetising
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Jobs
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Subscrictions
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Talent Workshops
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    CPSC Certificates
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Talent Workshops
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Ratings
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Shop Help
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Contact Us
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li>
                                <h4>Sites</h4>
                            </li>
                            <li>
                                <a href="#">
                                    DC
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    MAD Magazine
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    DC Kids
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    TV
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    DC Universe
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    DC Power Visa
                                </a>
                            </li>
                        </ul>
                    </div>
                    <div>
                        <ul>
                            <li>
                                <h4>SHOP</h4>
                            </li>
                            <li>
                                <a href="#">
                                    Shop DC
                                </a>
                            </li>
                            <li>
                                <a href="#">
                                    Shop DC Collectibles
                                </a>
                            </li>
                        </ul>
                    </div>
                </div>
            </section>

            <!-- third section -->
            <section class="social-links">
                <div class="box-sign-up">
                    <a href="#">
                        SIGN-UP NOW
                    </a>
                </div>
                <div>
                    <ul>
                        <li class="box-follow-us">
                            <a href="#">
                                <b>
                                    FOLLOW US
                                </b>
                             </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../img/footer-facebook.png" alt="facebook">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../img/footer-periscope.png" alt="periscope">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../img/footer-pinterest.png" alt="pinterst">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../img/footer-twitter.png" alt="twitter">
                            </a>
                        </li>
                        <li>
                            <a href="#">
                                <img src="../img/footer-youtube.png" alt="youtube">
                            </a>
                        </li>
                    </ul>
                </div>
            </section>
        </div>
    </footer>
</template>

<style scoped>
.container {
  display: flex;
  justify-content: center;
  align-items: center;
  background-color: #303030;
}

img {
  max-width: 100%;
}

ul {
  list-style: none;
}

a {
  text-decoration: none;
  padding: 5px;
  color: #696969;
}

a:hover {
    color: aquamarine;
}

a:active {
    background-color: darkgreen;
}

header .box-header-img{
    width: 5%;
}

.box-container {
    width: 80%;
    height: 50%;
    display: flex;
    justify-content: space-between;
    align-items: center;
}

.header-container {
    height: 80px;
    background-color: white;
}

header .box-links-header {
    width: 80%;
}

header .box-links-header ul {
    display: flex;
    justify-content: space-between;
}

header ul {
  display: flex;
}

header ul li {
  margin-left: 10px;
}

.main-container {
    background-color: #696969;
}

footer .box-container {
    width: 100%;
    flex-direction: column;
    flex-wrap: wrap;
}

footer .box-container .footer-nav, footer .box-container .social-links {
    width: 80%;
    margin: 30px 0;
}

footer .footer-nav ul {
    display: flex;
    flex-wrap: wrap;
    justify-content: space-between;
}

footer .footer-nav li {
    width: calc(100% / 10);
}

footer .footer-nav a {
    display: flex;
    align-items: center;
    gap: 5px;
}

footer .footer-links {
    width: 100%;
}

footer .footer-links {
    background-image: url(../img/footer-bg.jpg);
    display: flex;
    justify-content: center;
    padding: 30px 0;
}

footer .footer-links .box-footer-links {
    width: 80%;
    display: flex;
    gap: 40px;
    background-image: url(../img/dc-logo-bg.png);
    background-repeat: no-repeat;
    background-position-x: right;
    background-size: 20%;
}

footer .footer-links h4 {
    color: white;
}

footer .social-links {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

footer .social-links ul {
    display: flex;
    justify-content: space-between;
    align-items: center;
    gap: 10px;
}

footer .social-links ul li {
    display: flex;
    justify-content: space-between;
    align-items: center;
}

footer .social-links .box-sign-up a {
    border: 1px solid #2c67c0;
    color: white;
}

footer .social-links .box-follow-us a {
    color: #2c67c0;
    font-style: italic;
    border: none;
}
</style>