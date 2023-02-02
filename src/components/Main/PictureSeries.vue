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
        <h3>{{ picture.title }}</h3>
        <p>{{ picture.text }}</p>
    </div>
</template>
<style scoped lang="scss">
.card-image {
    width: calc(100% / 3 - 2rem);
    margin: .5rem 1rem;

    img {
        width: 150px;
        height: 150px;
        object-fit: fill;
    }

    h3 {
        color: white;
        text-align: left;
        font-size: 15px;
        font-weight: 500;

    }
}
</style>