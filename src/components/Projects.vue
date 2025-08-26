<template>
  <section class="min-h-screen py-20 bg-gray-50" aria-labelledby="projects-heading">
    <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header Section -->
      <header class="text-center mb-16" role="banner">
        <div class="inline-flex p-3 bg-blue-50 rounded-full mb-6">
          <svg class="w-10 h-10 text-blue-700" fill="none" stroke="currentColor" viewBox="0 0 24 24" aria-hidden="true">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M19 11H5m14 0a2 2 0 012 2v6a2 2 0 01-2 2H5a2 2 0 01-2-2v-6a2 2 0 012-2m14 0V9a2 2 0 00-2-2M5 11V9a2 2 0 012-2m0 0V5a2 2 0 012-2h6a2 2 0 012 2v2M7 7h10" />
          </svg>
        </div>
        <h1
          id="projects-heading"
          class="text-4xl sm:text-5xl md:text-6xl font-extrabold text-gray-900 mb-4"
        >
          My Projects
        </h1>
        <p class="text-lg sm:text-xl text-gray-500 max-w-3xl mx-auto leading-relaxed">
          A showcase of my recent work - from web applications to design projects, each crafted with passion and attention to detail.
        </p>
        <div class="mt-6 flex justify-center">
          <div class="w-24 h-1 bg-blue-600 rounded-full" aria-hidden="true"></div>
        </div>
      </header>

      <!-- Projects Grid -->
      <div class="grid grid-cols-1 sm:grid-cols-2 lg:grid-cols-3 gap-6 lg:gap-8" role="list">
        <article
          v-for="(project, index) in filteredProjects"
          :key="project.id"
          class="group bg-white rounded-xl shadow-sm overflow-hidden hover:shadow-lg transition-all duration-300 transform hover:-translate-y-1 border border-gray-100"
          :class="{ 'sm:col-span-2 lg:col-span-1': index === 0 }"
          role="listitem"
        >
          <!-- Project Image -->
          <div class="relative overflow-hidden aspect-w-16 aspect-h-9">
            <img
              :src="project.image"
              :alt="`Screenshot of ${project.title}`"
              class="w-full h-full object-cover group-hover:scale-105 transition-transform duration-500 ease-out"
              loading="lazy"
            />
            <div
              class="absolute inset-0 bg-gradient-to-t from-gray-900/20 to-transparent opacity-0 group-hover:opacity-100 transition-opacity duration-300"
              aria-hidden="true"
            ></div>
            <div class="absolute top-4 right-4 opacity-0 group-hover:opacity-100 transition-opacity duration-300">
              <div class="bg-white/90 rounded-full p-2 shadow-sm">
                <svg class="w-5 h-5 text-gray-600" fill="none" stroke="currentColor" viewBox="0 0 24 24" aria-hidden="true">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14" />
                </svg>
              </div>
            </div>
          </div>

          <!-- Project Content -->
          <div class="p-6 sm:p-7">
            <div class="flex items-center justify-between mb-4">
              <h3
                class="text-xl sm:text-2xl font-semibold text-gray-900 group-hover:text-blue-700 transition-colors duration-300"
              >
                {{ project.title }}
              </h3>
              <div
                class="w-8 h-8 bg-blue-600 rounded-full flex items-center justify-center"
              >
                <span class="text-white text-sm font-semibold">{{ index + 1 }}</span>
              </div>
            </div>

            <p class="text-gray-600 text-sm sm:text-base mb-6 leading-relaxed line-clamp-3">
              {{ project.description }}
            </p>

            <!-- Technologies -->
            <div class="flex flex-wrap gap-2 mb-6">
              <span
                v-for="tech in project.technologies"
                :key="tech"
                class="px-3 py-1 bg-gray-50 text-gray-700 text-xs sm:text-sm rounded-full font-medium border border-gray-200 hover:border-blue-400 hover:bg-blue-50 transition-all duration-300"
              >
                {{ tech }}
              </span>
            </div>

            <!-- Action Buttons -->
            <div class="flex gap-4">
              <a
                :href="project.liveDemo || '#'"
                class="flex-1 flex items-center justify-center gap-2 bg-blue-600 text-white px-4 py-2 sm:px-6 sm:py-3 rounded-lg font-medium hover:bg-blue-700 transform hover:scale-105 transition-all duration-300 shadow-sm hover:shadow-md"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="View live demo of {{ project.title }}"
              >
                <svg class="h-4 w-4" fill="none" viewBox="0 0 24 24" stroke="currentColor" aria-hidden="true">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M10 6H6a2 2 0 00-2 2v10a2 2 0 002 2h10a2 2 0 002-2v-4M14 4h6m0 0v6m0-6L10 14" />
                </svg>
                Live Demo
              </a>
              <a
                :href="project.code || '#'"
                class="flex items-center justify-center gap-2 bg-gray-700 text-white px-4 py-2 sm:px-6 sm:py-3 rounded-lg font-medium hover:bg-gray-800 transform hover:scale-105 transition-all duration-300 shadow-sm hover:shadow-md"
                target="_blank"
                rel="noopener noreferrer"
                aria-label="View source code of {{ project.title }}"
              >
                <svg class="h-4 w-4" fill="currentColor" viewBox="0 0 20 20" aria-hidden="true">
                  <path fill-rule="evenodd"
                    d="M10 0C4.477 0 0 4.484 0 10.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0110 4.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.942.359.31.678.921.678 1.856 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0020 10.017C20 4.484 15.522 0 10 0z"
                    clip-rule="evenodd" />
                </svg>
                Code
              </a>
            </div>
          </div>
        </article>
      </div>

      <!-- Call to Action -->
      <footer class="text-center mt-16" role="contentinfo" aria-labelledby="cta-heading">
        <div class="bg-blue-600 rounded-xl p-8 text-white">
          <h2 id="cta-heading" class="text-2xl sm:text-3xl font-bold mb-4">Interested in working together?</h2>
          <p class="text-blue-100 text-sm sm:text-base mb-6">
            Let's discuss your next project and bring your ideas to life.
          </p>
          <a
            href="#contact"
            class="inline-flex items-center bg-white text-blue-600 px-6 py-3 sm:px-8 sm:py-3 rounded-lg font-semibold hover:bg-gray-100 transform hover:scale-105 transition-all duration-300 shadow-sm hover:shadow-md"
            aria-label="Contact me to discuss a project"
          >
            Get In Touch
          </a>
        </div>
      </footer>
    </div>
  </section>
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
          technologies: ['PHP', 'MySQL', 'JavaScript', 'OOP'],
          liveDemo: '#',
          code: '#'
        },
        {
          id: 2,
          title: 'JavaScript Project',
          description: 'Built a JavaScript app to track daily expenses and calculate monthly totals in real time.',
          image: 'https://cdn.shopify.com/app-store/listing_images/48f1ca1ba97b7f347120eff90274f2c0/desktop_screenshot/CO3-jcn0lu8CEAE=.png?height=720&width=1280',
          technologies: ['JavaScript', 'HTML', 'CSS', 'Chart.js'],
          liveDemo: '#',
          code: '#'
        },
        {
          id: 3,
          title: 'Algorithm Project',
          description: 'Created an algorithm-based chatbot to automatically respond to messages and fetch weather info in Cambodia.',
          image: 'https://core.telegram.org/file/464001858/11318/ahAJjwERIX8.164875/ce1372cbf73e3ea94e',
          technologies: ['JavaScript', 'Weather API', 'CSS'],
          liveDemo: '#',
          code: '#'
        },
        {
          id: 4,
          title: 'Web Design Project',
          description: 'Focused on clean design, consistent layout, and compatibility across mobile and desktop devices.',
          image: 'https://i0.wp.com/themes.svn.wordpress.org/cake-shop-bakery/2.3.6/screenshot.png',
          technologies: ['Vue.js', 'Tailwind CSS', 'Netlify'],
          liveDemo: '#',
          code: '#'
        },
        {
          id: 5,
          title: 'Figma Design Poster',
          description: 'This was my first Figma project, and it shows my creativity in visual communication.',
          image: 'https://d1csarkz8obe9u.cloudfront.net/posterpreviews/digital-marketing-advertisement-design-template-ca539ed28728e68f73cf8a8415a8a006_screen.jpg?ts=1662986770',
          technologies: ['HTML', 'CSS', 'Sass'],
          liveDemo: '#',
          code: '#'
        },
        {
          id: 6,
          title: 'Library Management',
          description: 'To build a fully functional Library Management System using Laravel. CRUD operations for books, borrowing management.',
          image: 'https://infyom.com/images/features/lms/book-requests.webp',
          technologies: ['React', 'Socket.io', 'Node.js', 'Redis'],
          liveDemo: '#',
          code: '#'
        }
      ],
      filter: ''
    }
  },
  computed: {
    filteredProjects() {
      return this.filter
        ? this.projects.filter(project =>
            project.title.toLowerCase().includes(this.filter.toLowerCase()) ||
            project.description.toLowerCase().includes(this.filter.toLowerCase()) ||
            project.technologies.some(tech => tech.toLowerCase().includes(this.filter.toLowerCase()))
          )
        : this.projects
    }
  }
}
</script>

<style scoped>
/* Font stack for professional typography */
:root {
  font-family: 'Inter', -apple-system, BlinkMacSystemFont, 'Segoe UI', Roboto, sans-serif;
}

/* Text truncation for descriptions */
.line-clamp-3 {
  display: -webkit-box;
  -webkit-line-clamp: 3;
  -webkit-box-orient: vertical;
  overflow: hidden;
}

/* Responsive typography and spacing */
@screen sm {
  .text-4xl {
    font-size: 2.25rem;
  }
  .text-xl {
    font-size: 1.125rem;
  }
  .p-6 {
    padding: 1.5rem;
  }
}

@screen md {
  .text-5xl {
    font-size: 3rem;
  }
}

@screen lg {
  .text-6xl {
    font-size: 3.75rem;
  }
}

/* Accessibility: Focus styles */
a:focus, button:focus {
  outline: none;
  box-shadow: 0 0 0 3px rgba(59, 130, 246, 0.3);
}

/* Smooth scrolling */
html {
  scroll-behavior: smooth;
}

/* Image aspect ratio */
.aspect-w-16 {
  position: relative;
  padding-bottom: 56.25%; /* 16:9 aspect ratio */
}
.aspect-w-16 > img {
  position: absolute;
  top: 0;
  left: 0;
  width: 100%;
  height: 100%;
}

/* Subtle animations */
.group:hover .group-hover\:scale-105 {
  transform: scale(1.05);
}

/* Card hover effects */
article {
  transition: transform 0.3s ease-out, box-shadow 0.3s ease-out;
}
article:hover {
  transform: translateY(-4px);
}

/* Button hover effects */
a {
  transition: background-color 0.3s ease, transform 0.3s ease, box-shadow 0.3s ease;
}

/* Consistent border radius */
.rounded-lg {
  border-radius: 0.5rem;
}
.rounded-xl {
  border-radius: 0.75rem;
}
</style>