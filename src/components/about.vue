<template>
  <div class="min-h-screen py-20 bg-gradient-to-br from-blue-50 via-white to-purple-50">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header Section -->
      <div class="text-center mb-20">
        <div class="inline-block p-3 bg-gradient-to-r from-blue-100 to-purple-100 rounded-full mb-6">
          <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
          </svg>
        </div>
        <h1 class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-blue-600 via-purple-600 to-blue-800 bg-clip-text text-transparent mb-6">
          About Me
        </h1>
        <p class="text-xl text-gray-600 max-w-2xl mx-auto">
          Get to know me better - my journey, passion, and vision for the future
        </p>
        <div class="mt-8 flex justify-center">
          <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-purple-500 rounded-full"></div>
        </div>
      </div>

      <!-- Main Story Section -->
      <div class="grid md:grid-cols-2 gap-16 items-center mb-20">
        <div class="relative group">
          <div class="absolute -inset-4 bg-gradient-to-r from-blue-500 to-purple-500 rounded-2xl blur opacity-25 group-hover:opacity-40 transition duration-1000"></div>
          <div class="relative">
            <img
              src="https://lh3.googleusercontent.com/a/ACg8ocKWjVYrl9vRcndoB_SR0oTIUA0V0ddyb3NS6-_l2ZaoXxLEXQNQ=s360-c-no"
              alt="About me" 
              class="w-full rounded-2xl shadow-2xl transform group-hover:scale-105 transition duration-500"
            />
            <div class="absolute -bottom-6 -right-6 bg-white rounded-2xl p-4 shadow-xl">
              <div class="flex items-center space-x-2">
                <div class="w-3 h-3 bg-green-500 rounded-full animate-pulse"></div>
                <span class="text-sm font-semibold text-gray-700">Available for projects</span>
              </div>
            </div>
          </div>
        </div>
        
        <div class="space-y-6">
          <div class="inline-block px-4 py-2 bg-gradient-to-r from-blue-100 to-purple-100 rounded-full">
            <span class="text-blue-700 font-semibold text-sm">🎓 PNC Generation 2025</span>
          </div>
          
          <h2 class="text-3xl font-bold text-gray-900 mb-6">My Journey in Tech</h2>
          
          <div class="space-y-4">
            <div class="flex items-start space-x-4 p-4 bg-white rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
              <div class="w-8 h-8 bg-blue-100 rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                <svg class="w-4 h-4 text-blue-600" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z"/>
                </svg>
              </div>
              <p class="text-gray-600 leading-relaxed">
                I'm a passionate web development student at <strong class="text-blue-600">Passerelles numériques Cambodia (PNC)</strong> in generation 2025, where I've gained hands-on experience through collaborative team projects.
              </p>
            </div>

            <div class="flex items-start space-x-4 p-4 bg-white rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
              <div class="w-8 h-8 bg-purple-100 rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                <svg class="w-4 h-4 text-purple-600" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M13 6a3 3 0 11-6 0 3 3 0 016 0zM18 8a2 2 0 11-4 0 2 2 0 014 0zM14 15a4 4 0 00-8 0v3h8v-3z"/>
                </svg>
              </div>
              <p class="text-gray-600 leading-relaxed">
                Through <strong class="text-purple-600">4 major team projects</strong>, I've developed expertise in JavaScript applications, Telegram chatbots, responsive web design, and full-stack development using modern frameworks.
              </p>
            </div>

            <div class="flex items-start space-x-4 p-4 bg-white rounded-xl shadow-sm hover:shadow-md transition-shadow duration-300">
              <div class="w-8 h-8 bg-green-100 rounded-full flex items-center justify-center flex-shrink-0 mt-1">
                <svg class="w-4 h-4 text-green-600" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M11.49 3.17c-.38-1.56-2.6-1.56-2.98 0a1.532 1.532 0 01-2.286.948c-1.372-.836-2.942.734-2.106 2.106.54.886.061 2.042-.947 2.287-1.561.379-1.561 2.6 0 2.978a1.532 1.532 0 01.947 2.287c-.836 1.372.734 2.942 2.106 2.106a1.532 1.532 0 012.287.947c.379 1.561 2.6 1.561 2.978 0a1.533 1.533 0 012.287-.947c1.372.836 2.942-.734 2.106-2.106a1.533 1.533 0 01.947-2.287c1.561-.379 1.561-2.6 0-2.978a1.532 1.532 0 01-.947-2.287c.836-1.372-.734-2.942-2.106-2.106a1.532 1.532 0 01-2.287-.947zM10 13a3 3 0 100-6 3 3 0 000 6z" clip-rule="evenodd"/>
                </svg>
              </div>
              <p class="text-gray-600 leading-relaxed">
                My projects showcase versatility in both <strong class="text-green-600">front-end interfaces</strong> and <strong class="text-green-600">functional back-end systems</strong>, demonstrating my commitment to full-stack development excellence.
              </p>
            </div>
          </div>
        </div>
      </div>

      <!-- Experience Section -->
      <div class="mb-20">
        <div class="text-center mb-12">
          <h2 class="text-4xl font-bold text-gray-900 mb-4">Project Experience</h2>
          <p class="text-gray-600">Real-world projects that shaped my development journey</p>
        </div>
        
        <div class="space-y-6">
          <div v-for="(project, index) in projectExperience" :key="project.id" 
               class="group relative">
            <div class="flex items-start space-x-6 bg-white p-8 rounded-2xl shadow-lg hover:shadow-xl transition-all duration-500 transform hover:-translate-y-1">
              <div class="flex-shrink-0">
                <div class="w-16 h-16 bg-gradient-to-r from-blue-500 to-purple-500 rounded-2xl flex items-center justify-center text-white font-bold text-xl">
                  {{ index + 1 }}
                </div>
              </div>
              <div class="flex-grow">
                <div class="flex flex-col md:flex-row md:items-center md:justify-between mb-4">
                  <div>
                    <h3 class="text-2xl font-bold text-gray-900 group-hover:text-blue-600 transition-colors">
                      {{ project.title }}
                    </h3>
                    <p class="text-blue-600 font-semibold">{{ project.company }}</p>
                  </div>
                  <div class="flex items-center space-x-2 mt-2 md:mt-0">
                    <div class="px-3 py-1 bg-blue-100 text-blue-700 rounded-full text-sm font-medium">
                      {{ project.period }}
                    </div>
                  </div>
                </div>
                <p class="text-gray-600 leading-relaxed">{{ project.description }}</p>
                <div class="flex flex-wrap gap-2 mt-4">
                  <span v-for="tech in project.technologies" :key="tech"
                        class="px-3 py-1 bg-gray-100 text-gray-700 rounded-full text-sm font-medium">
                    {{ tech }}
                  </span>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>

      <!-- Education Section -->
      <div>
        <div class="text-center mb-12">
          <h2 class="text-4xl font-bold text-gray-900 mb-4">Education Journey</h2>
          <p class="text-gray-600">Building the foundation for my tech career</p>
        </div>
        
        <div class="grid md:grid-cols-2 gap-8">
          <div class="bg-gradient-to-br from-blue-50 to-blue-100 p-8 rounded-2xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-1">
            <div class="flex items-center mb-6">
              <div class="w-12 h-12 bg-blue-500 rounded-xl flex items-center justify-center mr-4">
                <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M10.394 2.08a1 1 0 00-.788 0l-7 3a1 1 0 000 1.84L5.25 8.051a.999.999 0 01.356-.257l4-1.714a1 1 0 11.788 1.838L7.667 9.088l1.94.831a1 1 0 00.787 0l7-3a1 1 0 000-1.838l-7-3zM3.31 9.397L5 10.12v4.102a8.969 8.969 0 00-1.05-.174 1 1 0 01-.89-.89 11.115 11.115 0 01.25-3.762zM9.3 16.573A9.026 9.026 0 007 14.935v-3.957l1.818.78a3 3 0 002.364 0l5.508-2.361a11.026 11.026 0 01.25 3.762 1 1 0 01-.89.89 8.968 8.968 0 00-5.35 2.524 1 1 0 01-1.4 0zM6 18a1 1 0 001-1v-2.065a8.935 8.935 0 00-2-.712V17a1 1 0 001 1z"/>
                </svg>
              </div>
              <div>
                <span class="inline-block px-3 py-1 bg-blue-200 text-blue-800 rounded-full text-xs font-semibold mb-2">
                  CURRENT
                </span>
              </div>
            </div>
            <h3 class="text-2xl font-bold text-gray-900 mb-2">Associate Degree</h3>
            <p class="text-blue-700 font-semibold mb-2">Passerelles Numériques Cambodia</p>
            <span class="text-blue-600 font-medium">2024 - Present</span>
            <p class="text-gray-600 mt-4 leading-relaxed">
              Intensive web development program focusing on modern technologies and real-world project experience.
            </p>
          </div>

          <div class="bg-gradient-to-br from-purple-50 to-purple-100 p-8 rounded-2xl shadow-lg hover:shadow-xl transition-all duration-300 transform hover:-translate-y-1">
            <div class="flex items-center mb-6">
              <div class="w-12 h-12 bg-purple-500 rounded-xl flex items-center justify-center mr-4">
                <svg class="w-6 h-6 text-white" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M6.267 3.455a3.066 3.066 0 001.745-.723 3.066 3.066 0 013.976 0 3.066 3.066 0 001.745.723 3.066 3.066 0 012.812 2.812c.051.643.304 1.254.723 1.745a3.066 3.066 0 010 3.976 3.066 3.066 0 00-.723 1.745 3.066 3.066 0 01-2.812 2.812 3.066 3.066 0 00-1.745.723 3.066 3.066 0 01-3.976 0 3.066 3.066 0 00-1.745-.723 3.066 3.066 0 01-2.812-2.812 3.066 3.066 0 00-.723-1.745 3.066 3.066 0 010-3.976 3.066 3.066 0 00.723-1.745 3.066 3.066 0 012.812-2.812zm7.44 5.252a1 1 0 00-1.414-1.414L9 10.586 7.707 9.293a1 1 0 00-1.414 1.414l2 2a1 1 0 001.414 0l4-4z" clip-rule="evenodd"/>
                </svg>
              </div>
              <div>
                <span class="inline-block px-3 py-1 bg-purple-200 text-purple-800 rounded-full text-xs font-semibold mb-2">
                  COMPLETED
                </span>
              </div>
            </div>
            <h3 class="text-2xl font-bold text-gray-900 mb-2">High School Diploma</h3>
            <p class="text-purple-700 font-semibold mb-2">Banlung Dormitory High School</p>
            <span class="text-purple-600 font-medium">2023 - 2024</span>
            <p class="text-gray-600 mt-4 leading-relaxed">
              Strong academic foundation with focus on mathematics and sciences, preparing for technology studies.
            </p>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'About',
  data() {
    return {
      projectExperience: [
        {
          id: 1,
          title: 'Grocery Store Management System',
          company: 'Team Project at PNC',
          period: 'Recent',
          description: 'Built a comprehensive grocery store management system using MVC architecture, featuring product display, shopping cart functionality, and sales tracking with modern UI/UX design.',
          technologies: ['PHP', 'MySQL', 'JavaScript', 'MVC', 'Figma']
        },
        {
          id: 2,
          title: 'JavaScript Expense Tracker',
          company: 'Personal Project',
          period: '2024',
          description: 'Developed a real-time expense tracking application with interactive charts and monthly calculations, demonstrating proficiency in vanilla JavaScript and data visualization.',
          technologies: ['JavaScript', 'HTML', 'CSS','Local Storage']
        },
        {
          id: 3,
          title: 'Telegram Chatbot',
          company: 'Algorithm Project',
          period: '2024',
          description: 'Created an intelligent chatbot using algorithmic responses to provide weather information for Cambodia, integrating external APIs and natural language processing.',
          technologies: ['JavaScript', 'Telegram API', 'Weather API', 'Algorithm Concept', 'CSS']
        },
        {
          id: 4,
          title: 'Responsive Bakery Website',
          company: 'Web Design Project',
          period: '2024',
          description: 'Designed and developed a fully responsive bakery website with clean aesthetics, ensuring cross-device compatibility and optimal user experience.',
          technologies: ['HTML', 'CSS', 'Sass', 'Responsive Design', 'JavaScript']
        }
      ]
    }
  }
}
</script>

<style scoped>
@keyframes float {
  0%, 100% { transform: translateY(0px); }
  50% { transform: translateY(-10px); }
}

.animate-float {
  animation: float 3s ease-in-out infinite;
}
</style>
