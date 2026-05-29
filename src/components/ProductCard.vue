<template>
    <div>
        <h1>Product card</h1>

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