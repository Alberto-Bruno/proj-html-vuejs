<script>
import pictureSeries from './PictureSeries.vue';
export default {
    components: {
        pictureSeries,
    },
    props: {
        Array,
    },
    data() {
        return {
            pictures: [
                {
                    image: '../../public/image/avada_01.jpg',
                    title: 'DJ Fusion',
                    text: 'August 19,2021@8.00 am',
                },
                {
                    image: '../../public/image/avada_02.jpg',
                    title: 'House Nation',
                    text: 'August 19,2021@8.00 am',
                },
                {
                    image: '../../public/image/avada_03.jpg',
                    title: 'Jazz Night',
                    text: "August 19,2021@8.00 am",
                },
                {
                    image: '../../public/image/avada_04.jpg',
                    title: 'VIP Taster Sessions',
                    text: 'August 19,2021@8.00 am',
                },
                {
                    image: '../../public/image/avada_05.jpg',
                    title: "Funky House Rave",
                    text: 'August 19,2021@8.00 am',
                },
                {
                    image: '../../public/image/avada_06.jpg',
                    title: "Urban Vibes",
                    text: 'August 19,2021@8.00 am',
                },
            ],
        }
    }
}
</script>

<template>
    <section>
        <div class="jumbo text-center text-white">
            <strong>SPECIAL EVENTS</strong>
            <h1>for your diary</h1>
            <div class="container p-5">
                <div class="row p-5">
                    <picture-series v-for="picture in pictures" :key="picture.image"
                        :picture="picture"></picture-series>
                </div>
                <button>RSVP NOW</button>
            </div>
        </div>
    </section>
    <section>
        <div class="slider">
            <div class="container">
                <div class="row p-5">
                    <div class="col text-center">
                        <strong>BECOME A VIP TONIGHT</strong>
                        <h1 class="text-white">exclusive vip lounge</h1>
                    </div>
                    <div class="col p-4 text-center">
                        <button>JOIN THE CLUB</button>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped lang="scss">
.jumbo {
    padding-top: 15%;
    width: 100%;
    min-height: 500px;
    background-image: url('../../assets/img/avada-nightclub-homepage-events-background-new.jpg');
    background-size: cover;

    button {
        padding: 10px 25px;
        background-color: #F63C81;
        color: white;
        font-size: 15px;
        font-weight: 600;
        cursor: pointer;
    }

    strong {
        color: #F63C81;
    }
}

.slider {
    width: 100%;
    min-height: 150px;
    background-image: url('../../assets/img/avada-nightclub-vip-hero-new.jpg');
    background-size: cover;

    button {
        padding: 10px 25px;
        background-color: #F63C81;
        color: white;
        font-size: 15px;
        font-weight: 600;
        cursor: pointer;
    }

    strong {
        color: #46b1fd;
    }
}
</style>