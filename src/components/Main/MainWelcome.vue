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
            <h4 class="dj-set-avada">dj avada</h4>
            <img src="../../assets/img/avada-nightclub-lisahouse-inset-new.jpg" alt="">
            <h4 class="dj-set-blondie">dj blondie</h4>
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

.dj-set-avada {
    position: absolute;
    left: 40px;
    padding: 50px;
    color: white;
}

.dj-set-blondie {
    position: absolute;
    left: 1000px;
    padding: 50px;
    color: white;
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