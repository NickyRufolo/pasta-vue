<template>
<div class="pasta-card">
    <img :src="propsPasta.img" alt="">
    <h2>{{propsPasta.tipo}}</h2>
</div>
</template>



<script>
export default {
    name: 'PastaCard',
    props: {
        propsPasta : Object
    }
}
</script>

<!-- Add "scoped" attribute to limit CSS to this component only -->
<style scoped lang="scss">
.pasta-card {
width: calc(( 100% / 5 ) - 20px );
border: 1px solid orange;
text-align: center;
margin: 10px 10px;
}
.pasta-card > img {
width: 100%;
}
</style>