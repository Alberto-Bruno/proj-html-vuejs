<script>
export default {
    props: {
        picture: Object,
    }
};
</script>

<template>
    <div class="card-image">
        <img :src="picture.image" :alt="picture.title">
        <h3><strong>{{ picture.title }}</strong></h3>
        <p><strong>{{ picture.text }}</strong></p>
    </div>
</template>
<style scoped lang="scss">
.card-image {
    width: calc(100% / 3 - 2rem);
    margin: .5rem 1rem;

    img {
        width: 280px;
        height: 150px;
    }

    h3 {
        color: #F63C81;
        text-align: left;
        font-size: 20px;
        font-weight: 600;
    }

    p {
        text-align: left;
        font-size: 15px;
    }
}
</style>