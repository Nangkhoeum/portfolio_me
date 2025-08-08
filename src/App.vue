<template>
  <div id="app">
    <!-- Enhanced Navigation Header -->
    <nav
      class="bg-gradient-to-r from-slate-900 via-slate-800 to-slate-900 shadow-xl fixed w-full top-0 z-50 backdrop-blur-sm">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="flex justify-between items-center h-20">
          <!-- Logo/Brand Section -->
          <div class="flex-shrink-0 flex items-center space-x-3">
            <div
              class="w-10 h-10 bg-gradient-to-br from-blue-400 to-purple-600 rounded-lg flex items-center justify-center shadow-lg">
              <span class="text-white font-bold text-xl">NC</span>
            </div>
            <div>
              <h1 class="text-2xl font-bold bg-gradient-to-r from-blue-400 to-purple-400 bg-clip-text text-transparent">
                NANGKHOEUM CHAMPHAI
              </h1>
              <p class="text-gray-400 text-xs tracking-wider">PROFESSIONAL PORTFOLIO</p>
            </div>
          </div>

          <!-- Desktop Navigation -->
          <div class="hidden md:block">
            <div class="ml-10 flex items-baseline space-x-2">
              <button v-for="page in pages" :key="page.id" @click="currentPage = page.id" :class="[
                'px-6 py-3 rounded-lg text-sm font-semibold transition-all duration-300 transform hover:scale-105 relative overflow-hidden group',
                currentPage === page.id
                  ? 'bg-gradient-to-r from-blue-500 to-purple-600 text-white shadow-lg'
                  : 'text-gray-300 hover:text-white hover:bg-white/10 backdrop-blur-sm'
              ]">
                <span class="relative z-10">{{ page.name }}</span>
                <div v-if="currentPage !== page.id"
                  class="absolute inset-0 bg-gradient-to-r from-blue-500/20 to-purple-600/20 opacity-0 group-hover:opacity-100 transition-opacity duration-300">
                </div>
              </button>
            </div>
          </div>

          <!-- Mobile menu button -->
          <div class="md:hidden">
            <button @click="mobileMenuOpen = !mobileMenuOpen"
              class="text-gray-300 hover:text-white focus:outline-none p-2 rounded-lg hover:bg-white/10 transition-colors duration-200">
              <svg class="h-6 w-6" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path v-if="!mobileMenuOpen" stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M4 6h16M4 12h16M4 18h16" />
                <path v-else stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M6 18L18 6M6 6l12 12" />
              </svg>
            </button>
          </div>
        </div>
      </div>

      <!-- Enhanced Mobile menu -->
      <div v-if="mobileMenuOpen" class="md:hidden transform transition-all duration-300">
        <div class="px-4 pt-4 pb-6 space-y-2 bg-slate-900/95 backdrop-blur-lg border-t border-slate-700">
          <button v-for="page in pages" :key="page.id" @click="currentPage = page.id; mobileMenuOpen = false" :class="[
            'block px-4 py-3 rounded-lg text-base font-medium w-full text-left transition-all duration-200 transform hover:scale-105',
            currentPage === page.id
              ? 'bg-gradient-to-r from-blue-500 to-purple-600 text-white shadow-lg'
              : 'text-gray-300 hover:text-white hover:bg-white/10'
          ]">
            {{ page.name }}
          </button>
        </div>
      </div>
    </nav>

    <!-- Main Content -->
    <main class="pt-20">
      <component :is="currentComponent" @navigate="navigateTo" />
    </main>

    <!-- Enhanced Professional Footer -->
    <footer class="bg-gradient-to-b from-slate-900 to-black text-white relative overflow-hidden">
      <!-- Background Pattern -->
      <div class="absolute inset-0 opacity-5">
        <div class="absolute top-0 left-0 w-full h-full"
          style="background-image: radial-gradient(circle at 2px 2px, white 1px, transparent 0); background-size: 40px 40px;">
        </div>
      </div>

      <div class="relative z-10">
        <!-- Main Footer Content -->
        <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-12">
          <div class="grid grid-cols-1 md:grid-cols-4 gap-8">

            <!-- Brand Column -->
            <div class="col-span-1 md:col-span-2">
              <div class="flex items-center space-x-3 mb-4">
                <div
                  class="w-12 h-12 bg-gradient-to-br from-blue-400 to-purple-600 rounded-xl flex items-center justify-center shadow-lg">
                  <span class="text-white font-bold text-xl">NC</span>
                </div>
                <div>
                  <h3
                    class="text-xl font-bold bg-gradient-to-r from-blue-400 to-purple-400 bg-clip-text text-transparent">
                    NANGKHOEUM CHAMPHAI
                  </h3>
                  <p class="text-gray-400 text-sm">Professional Portfolio</p>
                </div>
              </div>
              <p class="text-gray-400 leading-relaxed mb-6 max-w-md">
                Crafting digital experiences with passion and precision. Dedicated to creating innovative solutions that
                make a difference.
              </p>

              <!-- Social Links -->
              <div class="flex space-x-4">
                <a href="#"
                  class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-blue-500 transition-colors duration-300 group">
                  <svg class="w-5 h-5 text-gray-400 group-hover:text-white" fill="currentColor" viewBox="0 0 24 24">
                    <path
                      d="M24 4.557c-.883.392-1.832.656-2.828.775 1.017-.609 1.798-1.574 2.165-2.724-.951.564-2.005.974-3.127 1.195-.897-.957-2.178-1.555-3.594-1.555-3.179 0-5.515 2.966-4.797 6.045-4.091-.205-7.719-2.165-10.148-5.144-1.29 2.213-.669 5.108 1.523 6.574-.806-.026-1.566-.247-2.229-.616-.054 2.281 1.581 4.415 3.949 4.89-.693.188-1.452.232-2.224.084.626 1.956 2.444 3.379 4.6 3.419-2.07 1.623-4.678 2.348-7.29 2.04 2.179 1.397 4.768 2.212 7.548 2.212 9.142 0 14.307-7.721 13.995-14.646.962-.695 1.797-1.562 2.457-2.549z" />
                  </svg>
                </a>
                <a href="#"
                  class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-blue-600 transition-colors duration-300 group">
                  <svg class="w-5 h-5 text-gray-400 group-hover:text-white" fill="currentColor" viewBox="0 0 24 24">
                    <path
                      d="M20.447 20.452h-3.554v-5.569c0-1.328-.027-3.037-1.852-3.037-1.853 0-2.136 1.445-2.136 2.939v5.667H9.351V9h3.414v1.561h.046c.477-.9 1.637-1.85 3.37-1.85 3.601 0 4.267 2.37 4.267 5.455v6.286zM5.337 7.433c-1.144 0-2.063-.926-2.063-2.065 0-1.138.92-2.063 2.063-2.063 1.14 0 2.064.925 2.064 2.063 0 1.139-.925 2.065-2.064 2.065zm1.782 13.019H3.555V9h3.564v11.452zM22.225 0H1.771C.792 0 0 .774 0 1.729v20.542C0 23.227.792 24 1.771 24h20.451C23.2 24 24 23.227 24 22.271V1.729C24 .774 23.2 0 22.222 0h.003z" />
                  </svg>
                </a>
                <a href="#"
                  class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-gray-700 transition-colors duration-300 group">
                  <svg class="w-5 h-5 text-gray-400 group-hover:text-white" fill="currentColor" viewBox="0 0 24 24">
                    <path
                      d="M12 0c-6.626 0-12 5.373-12 12 0 5.302 3.438 9.8 8.207 11.387.599.111.793-.261.793-.577v-2.234c-3.338.726-4.033-1.416-4.033-1.416-.546-1.387-1.333-1.756-1.333-1.756-1.089-.745.083-.729.083-.729 1.205.084 1.839 1.237 1.839 1.237 1.07 1.834 2.807 1.304 3.492.997.107-.775.418-1.305.762-1.604-2.665-.305-5.467-1.334-5.467-5.931 0-1.311.469-2.381 1.236-3.221-.124-.303-.535-1.524.117-3.176 0 0 1.008-.322 3.301 1.23.957-.266 1.983-.399 3.003-.404 1.02.005 2.047.138 3.006.404 2.291-1.552 3.297-1.23 3.297-1.23.653 1.653.242 2.874.118 3.176.77.84 1.235 1.911 1.235 3.221 0 4.609-2.807 5.624-5.479 5.921.43.372.823 1.102.823 2.222v3.293c0 .319.192.694.801.576 4.765-1.589 8.199-6.086 8.199-11.386 0-6.627-5.373-12-12-12z" />
                  </svg>
                </a>
                <a href="#"
                  class="w-10 h-10 bg-white/10 rounded-lg flex items-center justify-center hover:bg-red-500 transition-colors duration-300 group">
                  <svg class="w-5 h-5 text-gray-400 group-hover:text-white" fill="currentColor" viewBox="0 0 24 24">
                    <path
                      d="M12.017 0C5.396 0 .029 5.367.029 11.987c0 5.079 3.158 9.417 7.618 11.174-.105-.949-.199-2.403.041-3.439.219-.937 1.406-5.957 1.406-5.957s-.359-.72-.359-1.781c0-1.663.967-2.911 2.168-2.911 1.024 0 1.518.769 1.518 1.688 0 1.029-.653 2.567-.992 3.992-.285 1.193.6 2.165 1.775 2.165 2.128 0 3.768-2.245 3.768-5.487 0-2.861-2.063-4.869-5.008-4.869-3.41 0-5.409 2.562-5.409 5.199 0 1.033.394 2.143.889 2.749.099.12.112.225.085.345-.09.375-.293 1.199-.334 1.363-.053.225-.172.271-.402.165-1.495-.69-2.433-2.878-2.433-4.646 0-3.776 2.748-7.252 7.92-7.252 4.158 0 7.392 2.967 7.392 6.923 0 4.135-2.607 7.462-6.233 7.462-1.214 0-2.357-.629-2.748-1.378 0 0-.599 2.282-.744 2.84-.282 1.084-1.064 2.456-1.549 3.235C9.584 23.815 10.77 24.001 12.017 24.001c6.624 0 11.99-5.367 11.99-11.988C24.007 5.367 18.641.001 12.017.001z" />
                  </svg>
                </a>
              </div>
            </div>

            <!-- Quick Links -->
            <div>
              <h4 class="text-lg font-semibold mb-4 text-white">Quick Links</h4>
              <ul class="space-y-2">
                <li v-for="page in pages" :key="page.id">
                  <button @click="navigateTo(page.id)"
                    class="text-gray-400 hover:text-blue-400 transition-colors duration-200 text-left">
                    {{ page.name }}
                  </button>
                </li>
              </ul>
            </div>

            <!-- Contact Info -->
            <div>
              <h4 class="text-lg font-semibold mb-4 text-white">Get In Touch</h4>
              <div class="space-y-3">
                <div class="flex items-center space-x-3">
                  <div class="w-8 h-8 bg-blue-500/20 rounded-lg flex items-center justify-center">
                    <svg class="w-4 h-4 text-blue-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                    </svg>
                  </div>
                  <span class="text-gray-400 text-sm">cpnkhoeumvd030005@gmail.com</span>
                </div>
                <div class="flex items-center space-x-3">
                  <div class="w-8 h-8 bg-green-500/20 rounded-lg flex items-center justify-center">
                    <svg class="w-4 h-4 text-green-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                    </svg>
                  </div>
                  <span class="text-gray-400 text-sm">088 468 3201</span>
                </div>
                <div class="flex items-center space-x-3">
                  <div class="w-8 h-8 bg-purple-500/20 rounded-lg flex items-center justify-center">
                    <svg class="w-4 h-4 text-purple-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                    </svg>
                  </div>
                  <span class="text-gray-400 text-sm">Phnom Penh, Cambodia</span>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Bottom Footer -->
        <div class="border-t border-gray-800">
          <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-6">
            <div class="flex flex-col md:flex-row justify-between items-center">
              <div class="text-gray-400 text-sm mb-4 md:mb-0">
                © 2025 Nangkhoeum Champhai. All rights reserved.
              </div>
              <div class="flex space-x-6 text-sm">
                <a href="#" class="text-gray-400 hover:text-blue-400 transition-colors duration-200">Privacy Policy</a>
                <a href="#" class="text-gray-400 hover:text-blue-400 transition-colors duration-200">Terms of
                  Service</a>
                <a href="#" class="text-gray-400 hover:text-blue-400 transition-colors duration-200">Sitemap</a>
              </div>
            </div>
          </div>
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
      this.mobileMenuOpen = false
    }
  }
}
</script>