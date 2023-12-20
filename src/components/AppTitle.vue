<script>
export default {
    data() {
        return {
            imageName: "vue.svg"
        }
    },
    methods: {
        getImagePath: function (imgPath) {
            return new URL(imgPath, import.meta.url).href;
        }
    }
};

</script>

<template>
    <h1 class="read-the-docs">La mia prima app con Vite!</h1>
    <img class="img" :src="getImagePath(`../assets/${imageName}`)" alt="vue">
</template>

<style scoped>
.read-the-docs {
    color: #888;
}

.img {
    width: 100px;
}
</style>
