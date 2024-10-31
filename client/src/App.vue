<template>
  <div class="flex">
    <Sidebar />
    <div class="flex-1">
      <Header />
      <MainContent />
    </div>
  </div>
</template>

<script>
import Sidebar from './components/AppSidebar.vue'
import Header from './components/AppHeader.vue'
import MainContent from './components/MainContent.vue'

export default {
  components: {
    Sidebar,
    Header,
    MainContent,
  },
}
</script>
