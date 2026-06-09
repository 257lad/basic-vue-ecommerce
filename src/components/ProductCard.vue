<template>
    <div>
        <h1>Product card</h1>
        <img src="https://lh5.googleusercontent.com/proxy/QeHvIzT_HtTkZEJKXMtYu5ryCYOJv-T-mzqCJnz-slG2IctXgspilg9tEn63hXQCYo3oioo0F4p8vvGq3jvlo1l4aM9l48ETh_qEbRoFc882ydA8Gw" alt="" width="200px" height="200px">
        <p>Image src: {{ item.img }}</p>
        <h4>Name {{ item.name }}</h4>
        <h4>Price {{ item.price }}</h4>
    </div>
</template>
<script>
export default {
    props: ['item']
}
</script>
<style scoped>

</style>