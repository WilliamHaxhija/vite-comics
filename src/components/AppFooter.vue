<script>
import AppFooterSocial from './AppFooterSocial.vue';
export default {
    name: 'AppFooter',
    components: {
        AppFooterSocial
    }
}
</script>

<template>
    <footer>
        <div class="container">
            <div class="links">
                <div>
                    <ul>
                        <li><a class="list-head" href="#">DC COMICS</a></li>
                        <li><a href="#">Characters</a></li>
                        <li><a href="#">Comics</a></li>
                        <li><a href="#">Movies</a></li>
                        <li><a href="#">TV</a></li>
                        <li><a href="#">Games</a></li>
                        <li><a href="#">Videos</a></li>
                        <li><a href="#">News</a></li>
                    </ul>
                    <ul>
                        <li><a class="list-head" href="#">SHOP</a></li>
                        <li><a href="#">Shop DC</a></li>
                        <li><a href="#">SHop DC Collectibles</a></li>
                    </ul>
                </div>
                <ul>
                    <li><a class="list-head" href="#">DC</a></li>
                    <li><a href="#">Terms Of Use</a></li>
                    <li><a href="#">Privacy policy (New)</a></li>
                    <li><a href="#">Add Choices</a></li>
                    <li><a href="#">Advertising</a></li>
                    <li><a href="#">Jobs</a></li>
                    <li><a href="#">Subscriptions</a></li>
                    <li><a href="#">Talent Workshops</a></li>
                    <li><a href="#">CPSC Certificates</a></li>
                    <li><a href="#">Ratings</a></li>
                    <li><a href="#">Shop Help</a></li>
                    <li><a href="#">Contact Us</a></li>
                </ul>
                <ul>
                    <li><a class="list-head" href="#">SITES</a></li>
                    <li><a href="#">DC</a></li>
                    <li><a href="#">MAD Magazine</a></li>
                    <li><a href="#">DC Kids</a></li>
                    <li><a href="#">DC Universe</a></li>
                    <li><a href="#">DC Power Visa</a></li>
                </ul>
            </div>
            <div class="big-logo"></div>
        </div>
        <AppFooterSocial></AppFooterSocial>
    </footer>
</template>

<style scoped lang="scss">
@use '../style/generic' as *;

footer {
    background-image: url('../assets/img/footer-bg.jpg');
    background-repeat: no-repeat;
    background-size: cover;
}

.container {
    display: flex;
    justify-content: space-between;

    .big-logo {
        background-image: url('../assets/img/dc-logo-bg.png');
        background-repeat: no-repeat;
        background-size: cover;
        background-position-y: -100px;
        height: 473px;
        width: 50%;
    }

    .links {
        display: flex;
        gap: 2rem;
        padding: 1rem 0;
    }

    ul {
        color: #959595;
        list-style: none;
        margin-top: 2rem;

        li {
            margin: 0.5rem 0;
        }

        a {
            color: #959595;
            text-decoration: none;

            &:hover {
                color: white;
                transition: 0.2s;
            }
        }

        .list-head {
            color: white;
            font-size: 1.2rem;
            font-weight: 700;
        }

        li:first-child {
            margin-bottom: 1rem;
        }
    }
}
</style>