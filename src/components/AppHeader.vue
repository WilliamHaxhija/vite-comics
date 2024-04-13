<script>
    export default {
        name: 'AppHeader',
        data() {
            return {
                navLinks: [
                    {
                        text: 'CHARACTERS',
                        active: false
                    },
                    {
                        text: 'COMICS',
                        active: false
                    },
                    {
                        text: 'MOVIES',
                        active: false
                    },
                    {
                        text: 'TV',
                        active: false
                    },
                    {
                        text: 'GAMES',
                        active: false
                    },
                    {
                        text: 'COLLECTIBLES',
                        active: false
                    },
                    {
                        text: 'VIDEOS',
                        active: false
                    },
                    {
                        text: 'FANS',
                        active: false
                    },
                    {
                        text: 'NEWS',
                        active: false
                    },
                    {
                        text: 'SHOP',
                        active: false
                    }
                ],
                activeLink: 0,
                isActive: false
            }
        },
        methods: {
            activateLink(index) {
                this.activeLink = index;
            }
        }
    }
</script>

<template>
    <header>
        <div class="container">
            <div>
            <img src="../assets/img/dc-logo.png" alt="logo">
        </div>
        <nav>
            <ul>
                <li v-for="link, index in navLinks" :class="{active: activeLink === index}">
                    <a href="#" @click="activateLink(index)">{{ link.text }}</a>
                </li>
            </ul>
        </nav>
        </div>
    </header>
</template>

<style scoped lang="scss">
    
    @use '../style/partials/variables' as *;

    header {
        background-color: white;
    }

    .container {
        display: flex;
        justify-content: space-between;
        align-items: center;
    }

    a {
        text-decoration: none;
        font-weight: 700;
        color: #464646;

        &:hover {
            color: $brand-primary;
        }

    }

    ul {
        list-style: none;
        display: flex;

        li {
            margin: 0 0.9rem;
            height: 9rem;
            position: relative;
            display: flex;
            align-items: center;
        }

        .active a {
            color: $brand-primary;
        }

        .active::after {
                content: '';
                width: 100%;
                height: 5px;
                background-color: $brand-primary;
                position: absolute;
                bottom: 0;
                left: 0;
            }
    }
</style>