<script>
export default {
    data() {

    }
}
</script>

<template>
    <div class="jumbo d-flex align-items-center justify-content-center text-center">
        <header class="container">
            <strong>WELCOME TO AVADA</strong>
            <h1 class="text-white">Have the night of your life</h1>
            <p class="w-50 mx-auto d-block text-white p-5">Lorem ipsum dolor sit amet consectetur adipisicing elit.
                Natus
                doloremsoluta
                eadoloresa, incidunt qui labore aut nam id, quisquam quas corrupti? Deserunt temporibus facilis eius
                nobis quae at.
            </p>
            <div class="row d-block text-white">
                <img src="../../assets/img/avada-nightclub-dancelounge-small.jpg" alt="">
                <img src="../../assets/img/avada-nightclub-rooftoplounge-small.jpg" alt="">
                <img src="../../assets/img/avada-nightclub-viplounge-small.jpg" alt="">
                <img src="../../assets/img/avada-nightclub-events-small.jpg" alt="">
            </div>
        </header>

    </div>
    <main class="container-fluid">
        <div class="row">
            <img class="image-dj" src="../../assets/img/avada-nightclub-resident-profile.jpg" alt="">
            <img src="../../assets/img/avada-nightclub-lisahouse-inset-new.jpg" alt="">
        </div>
    </main>
</template>

<style scoped lang="scss">
@use '../../assets/Styles/variables.scss' as*;
@use '../../assets/Styles/style.scss' as*;

.jumbo {
    background-image: url('../../assets/img/avada-nightclub-cloud-background.jpg');
    width: 100%;
    min-height: 1400px;
    background-size: cover;

    img {
        width: 40%;
        height: 400px;
    }

    strong {
        color: #46b1fd;
    }
}

img {
    width: 50%;

    &:hover {
        border-top: $border-top;
    }

    a:hover {
        color: $color-blue;
    }

}

.image-dj {
    width: 50%;

    &:hover {
        border-top: $border-bottom;
    }

    a:hover {
        color: $color-violet;
    }
}
</style>