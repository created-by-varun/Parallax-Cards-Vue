<template>
    <div class="product">
        <div class="product-inner">
            <div class="product-text-wrap">
                <h2 class="bg-text">
                    {{product.bgtext}}
                </h2>
            </div>
            <div class="product-image-wrap">
                <img :src="product.src" class="image" alt="">
            </div>
        </div>
    </div>
</template>

<script>
export default {
    name: 'product',
    props: ['product']
}
</script>