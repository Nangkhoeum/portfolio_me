<template>
  <div class="min-h-screen py-20 bg-gradient-to-br from-gray-50 to-white">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header Section -->
      <div class="text-center mb-20">
        <div class="inline-block p-2 bg-blue-100 rounded-full mb-6">
          <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
          </svg>
        </div>
        <h1
          class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-gray-900 via-blue-900 to-gray-900 bg-clip-text text-transparent mb-6">
          My Projects
        </h1>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto leading-relaxed">
          A showcase of my recent work - from web applications to design projects, each crafted with passion and
          attention to detail
        </p>
        <div class="mt-8 flex justify-center">
          <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full"></div>
        </div>
      </div>

      <!-- Projects Grid -->
      <div class="grid md:grid-cols-2 lg:grid-cols-3 gap-8">
        <div v-for="(project, index) in projects" :key="project.id"
          class="group bg-white rounded-2xl shadow-lg overflow-hidden hover:shadow-2xl transition-all duration-500 transform hover:-translate-y-2 border border-gray-100"
          :class="{ 'md:col-span-2 lg:col-span-1': index === 0 }">
          <!-- Project Image -->
          <div class="relative overflow-hidden">
            <img :src="project.image" :alt="project.title"
              class="w-full h-56 object-cover group-hover:scale-110 transition-transform duration-700" />
            <div
              class="absolute inset-0 bg-gradient-to-t from-black/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300">
            </div>
            <div class="absolute top-4 right-4 opacity-0 group-hover:opacity-100 transition-opacity duration-300">
              <div class="bg-white/90 backdrop-blur-sm rounded-full p-2">
                <svg class="w-5 h-5 text-gray-700" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14" />
                </svg>
              </div>
            </div>
          </div>

          <!-- Project Content -->
          <div class="p-8">
            <div class="flex items-center justify-between mb-4">
              <h3 class="text-2xl font-bold text-gray-900 group-hover:text-blue-600 transition-colors duration-300">
                {{ project.title }}
              </h3>
              <div
                class="w-8 h-8 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full flex items-center justify-center">
                <span class="text-white text-sm font-bold">{{ index + 1 }}</span>
              </div>
            </div>

            <p class="text-gray-600 mb-6 leading-relaxed line-clamp-3">
              {{ project.description }}
            </p>

            <!-- Technologies -->
            <div class="flex flex-wrap gap-2 mb-6">
              <span v-for="tech in project.technologies" :key="tech" v-if="tech"
                class="px-4 py-2 bg-gradient-to-r from-gray-100 to-gray-50 text-gray-700 text-sm rounded-full font-medium border border-gray-200 hover:border-blue-300 hover:bg-blue-50 transition-all duration-300">
                {{ tech }}
              </span>
            </div>

            <!-- Action Buttons -->
            <div class="flex gap-4">
              <button
                class="flex-1 flex items-center justify-center gap-2 bg-gradient-to-r from-blue-600 to-blue-700 text-white px-6 py-3 rounded-xl font-semibold hover:from-blue-700 hover:to-blue-800 transform hover:scale-105 transition-all duration-300 shadow-lg hover:shadow-xl">
                <svg class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14" />
                </svg>
                Live Demo
              </button>
              <button
                class="flex items-center justify-center gap-2 bg-gray-900 text-white px-6 py-3 rounded-xl font-semibold hover:bg-gray-800 transform hover:scale-105 transition-all duration-300 shadow-lg hover:shadow-xl">
                <svg class="h-4 w-4" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd"
                    d="M10 0C4.477 0 0 4.484 0 10.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0110 4.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.942.359.31.678.921.678 1.856 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0020 10.017C20 4.484 15.522 0 10 0z"
                    clip-rule="evenodd" />
                </svg>
                Code
              </button>
            </div>
          </div>
        </div>
      </div>

      <!-- Call to Action -->
      <div class="text-center mt-20">
        <div class="bg-gradient-to-r from-blue-600 to-purple-600 rounded-2xl p-8 text-white">
          <h3 class="text-2xl font-bold mb-4">Interested in working together?</h3>
          <p class="text-blue-100 mb-6">Let's discuss your next project and bring your ideas to life</p>
          <button
            class="bg-white text-blue-600 px-8 py-3 rounded-xl font-semibold hover:bg-gray-100 transform hover:scale-105 transition-all duration-300 shadow-lg">
            Get In Touch
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Projects',
  data() {
    return {
      projects: [
        {
          id: 1,
          title: 'Visual Company One',
          description: 'Developed a web system to display grocery products, manage a shopping cart, and track sales.',
          image: 'https://www.salesplay.com/wp-content/uploads/2022/01/Grocery-desktop.png',
          technologies: ['PHP', 'MySQL', 'JavaScript', 'OOP']
        },
        {
          id: 2,
          title: 'JavaScript Project',
          description: 'Built a JavaScript app to track daily expenses and calculate monthly totals in real time.',
          image: 'https://cdn.shopify.com/app-store/listing_images/48f1ca1ba97b7f347120eff90274f2c0/desktop_screenshot/CO3-jcn0lu8CEAE=.png?height=720&width=1280',
          technologies: ['JavaScript', 'HTML', 'CSS', 'Chart.js']
        },
        {
          id: 3,
          title: 'Algorithm Project',
          description: 'Created an algorithm-based chatbot to automatically respond to messages and fetch weather info in Cambodia.',
          image: 'https://core.telegram.org/file/464001858/11318/ahAJjwERIX8.164875/ce1372cbf73e3ea94e',
          technologies: ['JavaScript', 'Weather API', 'CSS']
        },
        {
          id: 4,
          title: 'Web Design Project',
          description: 'Focused on clean design, consistent layout, and compatibility across mobile and desktop devices.',
          image: 'https://i0.wp.com/themes.svn.wordpress.org/cake-shop-bakery/2.3.6/screenshot.png',
          technologies: ['Vue.js', 'Tailwind CSS', 'Netlify']
        },
        {
          id: 5,
          title: 'Figma Design Poster',
          description: 'This was my first Figma project, and it shows my creativity in visual communication. ',
          image: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/digital-marketing-advertisement-design-template-ca539ed28728e68f73cf8a8415a8a006_screen.jpg?ts=1662986770',
          technologies: ['HTML', 'CSS', 'Sass']
        },
        {
          id: 6,
          title: 'Library Management',
          description: 'To build a fully functional Library Management System using Laravel.CRUD operations for books, borrowing management.',
          image: 'https://infyom.com/images/features/lms/book-requests.webp',
          technologies: ['React', 'Socket.io', 'Node.js', 'Redis']
        }
      ]
    }
  }
}
</script>

<style scoped>
.line-clamp-3 {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}
</style>
