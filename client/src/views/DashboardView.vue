<template>
  <div class="grid grid-cols-1 md:grid-cols-3 gap-4 p-8">
    <!-- Sales Distribution -->
    <div class="col-span-1 md:col-span-3 bg-white rounded-lg shadow-md p-6">
      <h3 class="text-lg font-semibold mb-2">Sales Distribution</h3>
      <p class="text-gray-500 mb-4">This is all over Platform Sales Generated</p>
      <div class="flex justify-between">
        <div class="text-center">
          <p class="text-2xl font-bold">$34,343.00</p>
          <p class="text-gray-500">Total Sales</p>
        </div>
        <div class="text-center">
          <p class="text-2xl font-bold">$4.5k</p>
          <p class="text-gray-500">By Website</p>
        </div>
        <div class="text-center">
          <p class="text-2xl font-bold">$2.8k</p>
          <p class="text-gray-500">By Mobile</p>
        </div>
        <div class="text-center">
          <p class="text-2xl font-bold">$2.2k</p>
          <p class="text-gray-500">By Market</p>
        </div>
        <div class="text-center">
          <p class="text-2xl font-bold">$1.7k</p>
          <p class="text-gray-500">By Agent</p>
        </div>
      </div>
    </div>

    <!-- Other Cards -->
    <div class="bg-white rounded-lg shadow-md p-6">
      <h3 class="text-lg font-semibold mb-2">Sales Overview</h3>
      <p class="text-xl font-bold text-center">$500,00</p>
    </div>
    <div class="bg-white rounded-lg shadow-md p-6">
      <h3 class="text-lg font-semibold mb-2">Revenue Updates</h3>
      <p class="text-center">Graph Placeholder</p>
    </div>
    <div class="bg-white rounded-lg shadow-md p-6">
      <h3 class="text-lg font-semibold mb-2">Yearly Sales</h3>
      <p class="text-center">Graph Placeholder</p>
    </div>
    <div class="bg-white rounded-lg shadow-md p-6">
      <h3 class="text-lg font-semibold mb-2">Active User</h3>
      <p class="text-center">Map Placeholder</p>
    </div>
    <div class="bg-white rounded-lg shadow-md p-6">
      <h3 class="text-lg font-semibold mb-2">Payment Gateways</h3>
      <ul>
        <li>Paypal: +$6235</li>
        <li>Wallet: -$235</li>
        <li>Credit card: +$2235</li>
      </ul>
    </div>
  </div>
</template>

<script>
export default {
  name: 'DashboardView',
}
</script>
