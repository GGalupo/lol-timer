<template>
    <img class="cdr" :src="resolve_url(src)" >
</template>

<script>
export default {
    props: {
        src: String
    },
    methods: {
        resolve_url: function(path) {
            let imgs = require.context('../assets/imgs', false, /\.png$|\.jpg$/)
            return imgs("./" + path)
        }
    }
}
</script>

<style>
.cdr {
    width: 20%;
    padding: 5px;
    -webkit-filter: grayscale(100%);
    filter: grayscale(100%);
}
</style>