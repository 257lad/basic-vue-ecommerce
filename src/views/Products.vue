<template>
    <h1>Products </h1>
    <div class="products-container">
        <Filter />
        <div class="cards-container">
            <ProductCard v-for="item in 8" :key="item.id" />
        </div>
    </div>
</template>
<script>
import Filter from '@/components/Filter.vue';
import ProductCard from '@/components/ProductCard.vue';

export default {

    components: {
        Filter,
        ProductCard
    }
}
</script>
<style scoped>
    .products-container {
        display: flex;
        gap: 30px
    }
    .cards-container {
        display: grid;
        grid-template-columns: 1fr 1fr 1fr 1fr;
        gap: 20px;
    }
</style>