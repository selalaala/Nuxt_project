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
                            <tr>
                                <td><img src="../assets/svg/asgard-sofa.svg" alt="Logo" class="asgard-sofa" />Asgaard sofa</td>
                                <td>Rp. 250,000.00</td>
                                <td>1</td>
                                <td>Rp. 250,000.00</td>
                                <td><i class="bi bi-trash trash"></i></td>
                            </tr>
                        </tbody>
                    </table>
                </div>
                <div class="col-lg-4">
                    <div class="card">
                        <div class="">
                            <h3 class="text-center">Cart Totals</h3>
                            <p>Subtotal: Rp. 250,000.00</p>
                            <p>Total:   Rp. 250,000.00</p>
                            <button class="btn"><NuxtLink to="/checkout" class="btn btn-outline-dark">Checkout</NuxtLink></button>
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
</style>