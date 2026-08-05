<template>
    <section>
        <div class="container">
            <div class="row">
                <div class="col-lg-8">
                    <table class="table">
                        <thead class="thead-light">
                            <tr>
                                <th>Product</th>
                                <th>Price</th>
                                <th>Quantity</th>
                                <th>Subtotal</th>
                                <th></th>
                            </tr>
                        </thead>
                        <tbody class="text-center">
                            <tr v-for="item in cartItems" :key="item.id">
                                <td>
                                    <img :src="item.image" :alt="item.name" class="asgard-sofa" />
                                    {{ item.name }}
                                </td>
                                <td>{{ item.price }}</td>
                                <td>{{ item.quantity }}</td>
                                <td>{{ item.subtotal }}</td>
                                <td>
                                    <i class="bi bi-trash trash"></i>
                                </td>
                            </tr>
                        </tbody>
                    </table>
                </div>
                <div class="col-lg-4">
                    <div class="card">
                        <div class="">
                            <h3 class="text-center">Cart Totals</h3>
                            <div class="d-flex justify-content-between mb-3">
                                <span>Subtotal</span>
                                <span class="text-secondary">Rp. {{ cartSummary.subtotal}}</span>
                            </div>
                            <div class="d-flex justify-content-between mb-3">
                                <span>Total</span>
                                <span class="text-warning">Rp. {{ cartSummary.total}}</span>
                            </div>
                            <div class="text-center">
                                <button class="btn">
                                    <NuxtLink to="/checkout" class="btn btn-outline-dark">Checkout</NuxtLink>
                                </button>
                            </div>
                        </div>
                    </div>
                </div>
            </div>
        </div>
    </section>
</template>

<style scoped>
.row {
    padding: 60px 0;
}

.card {
    background-color: #FFF3E3;
    padding: 20px 20px;
}

.asgard-sofa {
    width: 99px;
    margin-right: 10px;
}

.thead-light th {
    background-color: #FFF3E3;
    text-align: center;
}

.trash {
    color: #B88E2F;
    font-size: 20px;
    cursor: pointer;
}

.card {
    border: none;
    border-radius: 0;
    background-color: #FFF3E3;
}

@media (max-width: 576px) {
    .table {
        font-size: 12px;
    }

    .asgard-sofa {
        width: 60px;
        margin-right: 5px;
    }

    .table td,
    .table th {
        padding: 8px 4px;
    }
}
</style>

<script setup>
defineProps({
  cartItems: Array,
  cartSummary: Object
})
</script>