<template>
    <h1>Products </h1>
    <div class="products-container">
        <Filter />
        <div class="cards-container">
            <ProductCard v-for="value in products" :key="value.id" :item="value" />
        </div>
    </div>
</template>
<script>
import Filter from '@/components/Filter.vue';
import ProductCard from '@/components/ProductCard.vue';

export default {
    data() {
        return {
            products: [
                {
                    id: 1,
                    img: '--img-src-1',
                    name: 'product 1',
                    price: 0
                },
                {
                    id:2,
                    img: '--img-src-2',
                    name: 'product 2',
                    price: 1000
                },
            ]
        }
    },
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