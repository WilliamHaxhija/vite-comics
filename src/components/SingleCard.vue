<script>
export default {
    name: 'SingleCard',
    props: ['card']
}
</script>

<template>
    <div class="card">
        <div>
            <img :src="card.thumb" alt="comic">
        </div>
        <span>{{ card.series }}</span>
    </div>
</template>

<style scoped lang="scss">

    .card {
        color: rgb(237, 235, 235);
        flex-shrink: 0;
        flex-grow: 0;
        width: calc((100% / 6) - 2rem);
        margin-top: 1.3rem;
        cursor: pointer;

        &:hover {
            opacity: 0.8;
            transition: 0.2s;
        }

        img {
            width: 100%;
            height: 179px;
            object-fit: cover;
            margin-bottom: 1rem;
        }

        span {
            text-transform: uppercase;
            font-size: 0.9rem;
        }
    }

</style>