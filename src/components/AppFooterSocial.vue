<script>
export default {
    name: 'AppFooterSocial'
}
</script>
<template>
    <div class="background">
        <div class="container">
            <button>SIGN-UP NOW!</button>
            <div class="social">
                <span>FOLLOW US</span>
                <div class="sites">
                    <img src="../assets/img/footer-facebook.png" alt="facebook">
                    <img src="../assets/img/footer-twitter.png" alt="facebook">
                    <img src="../assets/img/footer-youtube.png" alt="facebook">
                    <img src="../assets/img/footer-pinterest.png" alt="facebook">
                    <img src="../assets/img/footer-periscope.png" alt="facebook">
                </div>
            </div>
        </div>
    </div>
</template>
<style scoped lang="scss">

@use '../style/generic' as *;

.background {
    background-color: #303030;
}

.container {
    display: flex;
    justify-content: space-between;
    padding: 1.5rem 0;

    .social {
        display: flex;
        align-items: center;
    }

    button {
        background-color: transparent;
        border-color: #0282f9;
        border-style: solid;
        color: white;
        font-size: 1rem;
        font-weight: 700;
        padding: 0.8rem;
        cursor: pointer;

        &:hover {
            transform: scale(1.05);
            transition: 0.2s;
        }
    }

    span {
        color: #1182f9;
        font-weight: 700;
        margin-right: 1.5rem;
    }

    .sites {
        img {
            margin-right: 1rem;

            &:hover {
                filter: invert(1);
                cursor: pointer;
            }
        }
    }
}

</style>