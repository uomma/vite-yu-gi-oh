<script>

export default {
    name: 'CartaCard',
    props: {
        img: String,
        title: String,
        type: String,
    }
}
</script>
<template>
    <article class="text-center">
        <div class="img"><img class="img-fluid" :src="img" alt="img"></div>
        <h2>{{ title }}</h2>
        <p>{{type}}</p>
    </article>
</template>


<style lang="scss" scoped>
article{
    background-color: orange;
    font-weight: 600;
}
h2{
    color: white;
}
</style>