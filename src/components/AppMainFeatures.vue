<script>

export default {
    name: 'AppMainFeatures'
}

</script>

<template>
    <section>
        <div class="container">
            <div class="features">
                <img src="../assets/img/buy-comics-digital-comics.png" alt="e-commerce">
                <span>DIGITAL COMICS</span>
            </div>
            <div class="features">
                <img src="../assets/img/buy-comics-merchandise.png" alt="e-commerce">
                <span>DC MERCHANDISE</span>
            </div>
            <div class="features">
                <img src="../assets/img/buy-comics-subscriptions.png" alt="e-commerce">
                <span>SUBSCRIPTIONS</span>
            </div>
            <div class="features">
                <img class="locator" src="../assets/img/buy-comics-shop-locator.png" alt="e-commerce">
                <span>COMIC SHOP LOCATOR</span>
            </div>
            <div class="features last">
                <img src="../assets/img/buy-dc-power-visa.svg" alt="e-commerce">
                <span>DC POWER VISA</span>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
@use '../style/generic';
@use '../style/partials/variables' as *;

section {
    background-color: $brand-primary;
    padding: 2.5rem 0;
}

.container {
    display: flex;
    justify-content: center;
    gap: 0.5rem;
    
}

.features {
    display: flex;
    align-items: center;
    justify-content: center;
    color: white;

    &.last {
        flex-grow: 1;

        img {
            max-width: 16.5%;
        }
    }

    img {
        max-width: 20%;

        &.locator {
            max-height: 59px;
            margin-left: 1rem;
        }
    }

    span {
        margin-left: 1rem;
        font-size: smaller;
    }
}
</style>