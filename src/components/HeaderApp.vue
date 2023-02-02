<script>
export default {
    data() {
        return {
            menu: [
                {
                    label: 'HOME',
                    url: '#',
                    active: true
                },
                {
                    label: 'THE CLUB',
                    url: '#',
                    active: false
                },
                {
                    label: 'EVENTS',
                    url: '#',
                    active: false
                },
                {
                    label: 'JOBS',
                    url: '#',
                    active: false
                },
                {
                    label: 'NEWS',
                    url: '#',
                    active: false
                },
                {
                    label: 'CONTACT US',
                    url: '#',
                    active: false
                },
            ],
        }
    }
}
</script>

<template>
    <div class="jumbo">
        <header class="container-fluid">
            <a href="">
                <img class="logo" src="../assets/img/avada-nightclub-logo.png" alt="NightClub logo">
            </a>
            <nav>
                <ul>
                    <li v-for="(item, index) in menu" :key="index" :class="item.active ? 'active' : ''">
                        <a :href="item.url">
                            <strong>{{ item.label }}</strong>
                        </a>
                    </li>
                </ul>
            </nav>
        </header>
        <div class="">
            <img class="img-nightclub mx-auto d-block" src="../assets/img/avada-nightclub-homepage-image-1200x596.png"
                alt="">
            <h2 class="bg-black text-center text-white shadow p-3 mb-5 bg-opacity-75 rounded mx-auto d-block ">
                Making
                memories all
                night
                long
            </h2>
            <button class="mx-auto d-block">BECOME A VIP</button>
        </div>
        <a href="#">
            <img class="mx-auto d-block p-4" src="../assets/img/avada-nightclub-play-showreel-200x47.png" alt="">
        </a>
    </div>
</template>

<style scoped lang="scss">
@use '../assets/Styles/variables.scss' as*;
@use '../assets/Styles/style.scss' as*;

.logo {
    width: 200px;
    margin-left: 100px;
}

.jumbo {
    background-image: url('../assets/img/avada-nightclub-home-hero.jpg');
    width: 100%;
    min-height: 500px;
    background-size: cover;

    h2 {
        width: 60%;
        border-top: 3px solid #46b1fd;
    }

    button {
        position: relative;
        bottom: 60px;
        padding: 10px 25px;
        background-color: #F63C81;
        color: white;
        font-size: 20px;
        cursor: pointer;
    }
}

header {
    display: flex;
    justify-content: space-around;
    align-items: center;

    nav {
        display: flex;
        align-items: center;
        height: 100%;

        ul {
            height: 100%;
            list-style: none;
            margin: 2rem 1rem;
            display: flex;
            align-items: center;

            li {
                height: 100%;
                padding: 1rem;
                font-size: 10px;
                font-family: 'Roboto', sans-serif;
                font-weight: 700;
                display: flex;
                align-items: center;

                &.active {
                    border-bottom: $border-bottom;

                    a {
                        color: $color-violet;
                    }
                }

                &:hover {
                    border-bottom: $border-bottom;
                }

                a:hover {
                    color: $color-violet;
                }
            }
        }

    }
}
</style>