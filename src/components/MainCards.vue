<script>
export default {
    props: {
        url_image: String,
        series_title: String
    }
}
</script>

<template>
    <div class="card p-0" style="width: calc(100%/4 );">
        <img class="card-img-top" :src="url_image" alt="Card image cap">
        <div class="card-body">
            <h5 class="card-title"> {{ series_title }} </h5>
        </div>
    </div>


</template>

<style lang="scss" scoped>
@use "../styles/partials/variables" as *;

div.card {
    margin: 0 3rem 4rem;

    div.card-body {
        background-color: $main-color;
        color: white;
    }
}
</style>