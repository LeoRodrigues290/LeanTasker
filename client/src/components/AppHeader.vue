<template>
  <header class="bg-white py-4 ml-64 px-8 shadow-md">
    <div class="px-8 flex justify-between items-center">
      <div class="flex items-center space-x-4">
        <h1 class="text-xl font-semibold">Dashboard</h1>
        <input
            type="text"
            placeholder="Search"
            class="px-4 py-2 rounded-lg border border-gray-200 focus:outline-none"
        />
      </div>
      <div class="flex items-center space-x-4">
        <button class="p-2 bg-gray-100 rounded-full hover:bg-gray-200">
          <!-- Ícone de notificação -->
          <i class="fas fa-bell"></i>
        </button>
        <button class="p-2 bg-gray-100 rounded-full hover:bg-gray-200">
          <!-- Ícone de configuração -->
          <i class="fas fa-cog"></i>
        </button>
      </div>
    </div>
  </header>
</template>

<script>
export default {
  name: 'AppHeader',
}
</script>
