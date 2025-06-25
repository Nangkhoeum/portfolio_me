<template>
  <div id="app">
    <!-- Navigation -->
    <nav class="bg-white shadow-sm fixed w-full top-0 z-50">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between items-center h-16">
          <div class="flex-shrink-0">
            <h1 class="text-xl font-bold text-gray-900">NANGKHOEUM CHAMPHAI</h1>
          </div>
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-4">
              <button
                v-for="page in pages"
                :key="page.id"
                @click="currentPage = page.id"
                :class="[
                  'px-3 py-2 rounded-md text-sm font-medium transition-colors',
                  currentPage === page.id
                    ? 'bg-gray-900 text-white'
                    : 'text-gray-700 hover:bg-gray-100'
                ]"
              >
                {{ page.name }}
              </button>
            </div>
          </div>
          <div class="md:hidden">
            <button
              @click="mobileMenuOpen = !mobileMenuOpen"
              class="text-gray-700 hover:text-gray-900 focus:outline-none"
            >
              <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M4 6h16M4 12h16M4 18h16" />
              </svg>
            </button>
          </div>
        </div>
      </div>
      
      <!-- Mobile menu -->
      <div v-if="mobileMenuOpen" class="md:hidden">
        <div class="px-2 pt-2 pb-3 space-y-1 sm:px-3 bg-white border-t">
          <button
            v-for="page in pages"
            :key="page.id"
            @click="currentPage = page.id; mobileMenuOpen = false"
            :class="[
              'block px-3 py-2 rounded-md text-base font-medium w-full text-left transition-colors',
              currentPage === page.id
                ? 'bg-gray-900 text-white'
                : 'text-gray-700 hover:bg-gray-100'
            ]"
          >
            {{ page.name }}
          </button>
        </div>
      </div>
    </nav>

    <!-- Main Content -->
    <main class="pt-16">
      <component :is="currentComponent" @navigate="navigateTo" />
    </main>

    <!-- Footer -->
    <footer class="bg-gray-900 text-white py-8">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center">
          <p class="text-gray-400">
            © 2024 John Doe. All rights reserved.
          </p>
        </div>
      </div>
    </footer>
  </div>
</template>

<script>
import Home from './components/Home.vue'
import About from './components/about.vue'
import Projects from './components/Projects.vue'
import Contact from './components/contact.vue'

export default {
  name: 'App',
  components: {
    Home,
    About,
    Projects,
    Contact
  },
  data() {
    return {
      currentPage: 'home',
      mobileMenuOpen: false,
      pages: [
        { id: 'home', name: 'Home' },
        { id: 'about', name: 'About' },
        { id: 'projects', name: 'Projects' },
        { id: 'contact', name: 'Contact' }
      ]
    }
  },
  computed: {
    currentComponent() {
      const componentMap = {
        home: 'Home',
        about: 'About',
        projects: 'Projects',
        contact: 'Contact'
      }
      return componentMap[this.currentPage] || 'Home'
    }
  },
  methods: {
    navigateTo(page) {
      this.currentPage = page
    }
  }
}
</script>
