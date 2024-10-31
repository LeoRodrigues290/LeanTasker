<template>
  <aside class="w-64 bg-gray-100 h-screen p-4 flex flex-col justify-between fixed">
    <div>
      <div class="text-lg font-semibold mb-6">Catalog</div>
      <nav class="space-y-4">
        <h2 class="text-gray-500 text-sm uppercase mb-2">Home</h2>
        <ul>
          <li>
            <router-link
                to="/"
                class="block py-2 px-4 rounded hover:bg-gray-200 cursor-pointer flex items-center space-x-2"
                :class="{'bg-blue-100 text-blue-500': $route.path === '/'}"
            >
              <i class="fas fa-home"></i>
              <span>Dashboard</span>
            </router-link>
          </li>
        </ul>
        <h2 class="text-gray-500 text-sm uppercase mb-2 mt-6">App</h2>
        <ul>
          <li v-for="(item, index) in appLinks" :key="index">
            <router-link
                :to="item.to"
                class="block py-2 px-4 rounded hover:bg-gray-200 cursor-pointer flex items-center space-x-2"
                :class="{'bg-blue-100 text-blue-500': $route.path === item.to}"
            >
              <i :class="item.icon"></i>
              <span>{{ item.label }}</span>
            </router-link>
          </li>
        </ul>
      </nav>
    </div>
    <div class="flex items-center space-x-3 p-4 bg-gray-200 rounded-lg mt-4">
      <img
          src="https://via.placeholder.com/40"
          alt="User Avatar"
          class="w-10 h-10 rounded-full"
      />
      <div>
        <p class="font-semibold">Jane Cooper</p>
        <p class="text-sm text-gray-500">Admin</p>
      </div>
    </div>
  </aside>
</template>

<script>
export default {
  name: 'AppSidebar',
  data() {
    return {
      appLinks: [
        { to: '/contacts', label: 'Contacts', icon: 'fas fa-address-book' },
        { to: '/chats', label: 'Chats', icon: 'fas fa-comments' },
        { to: '/calendar', label: 'Calendar', icon: 'fas fa-calendar-alt' },
        { to: '/email', label: 'Email', icon: 'fas fa-envelope' },
        { to: '/tickets', label: 'Tickets', icon: 'fas fa-ticket-alt' },
      ],
    }
  },
}
</script>

<style scoped>
/* Importando Font Awesome para os ícones */
@import url("https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.4/css/all.min.css");
</style>
