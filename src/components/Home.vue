<template>
  <div class="min-h-screen">
    <!-- Hero Section -->
    <section class="bg-gradient-to-r from-gray-900 to-gray-700 text-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8 py-24">
        <div class="text-center">
          <div class="mb-8">
            <img
              src="https://lh3.googleusercontent.com/a/ACg8ocKWjVYrl9vRcndoB_SR0oTIUA0V0ddyb3NS6-_l2ZaoXxLEXQNQ=s360-c-no"
              alt="Profile" class="w-32 h-32 rounded-full mx-auto mb-6 border-4 border-white shadow-lg" />
          </div>
          <h1 class="text-4xl md:text-6xl font-bold mb-6">
            Hi, I'm <span class="text-yellow-400">Nangkhoeum Champhai</span>
          </h1>
          <p class="text-xl md:text-2xl mb-8 text-gray-300">
            Web Student Development
          </p>
          <p class="text-lg mb-8 max-w-2xl mx-auto text-gray-400">

            I'm a student in web development at Passerelles numériques Cambodia (PNC) in generation 2025. I have many
            experiences related to projects at my school/PNC. I have worked as a team and built 4 projects.
          </p>
          <div class="flex flex-col sm:flex-row gap-4 justify-center">
            <button @click="$emit('navigate', 'projects')"
              class="bg-yellow-400 text-gray-900 px-8 py-3 rounded-lg font-semibold hover:bg-yellow-300 transition-colors">
              View My Work
            </button>
            <button @click="$emit('navigate', 'contact')"
              class="border-2 border-white text-white px-8 py-3 rounded-lg font-semibold hover:bg-white hover:text-gray-900 transition-colors">
              Get In Touch
            </button>
          </div>
        </div>
      </div>
    </section>

    <!-- Skills Section -->
    <section class="py-20 bg-white">
      <div class="max-w-7xl mx-auto px-4 sm:px-6 lg:px-8">
        <div class="text-center mb-16">
          <h2 class="text-3xl md:text-4xl font-bold text-gray-900 mb-4">Skills & Technologies</h2>
          <p class="text-lg text-gray-600">Technologies I have learn</p>
        </div>
        <div class="grid grid-cols-2 md:grid-cols-4 lg:grid-cols-6 gap-8">
          <div v-for="skill in skills" :key="skill"
            class="text-center p-6 bg-gray-50 rounded-lg hover:shadow-md transition-shadow">
            <div class="w-12 h-12 bg-gray-900 rounded-lg mx-auto mb-4 flex items-center justify-center">
              <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                  d="M10 20l4-16m4 4l4 4-4 4M6 16l-4-4 4-4" />
              </svg>
            </div>
            <h3 class="font-semibold text-gray-900">{{ skill }}</h3>
          </div>
        </div>
      </div>
    </section>
  </div>
</template>

<script>
export default {
  name: 'Home',
  emits: ['navigate'],
  data() {
    return {
      skills: [
        'Figma', 'GitHub', 'HTML/CSS', 'SASS', 'Web Design', 'Algorithm', 'JavaScript', 'MySQL', 'AWS', 'Wordpress',
        'OOP', 'TypeScript', 'PHP', 'Node.js', 'Vue.js', 'Bootstrap', 'Tailwind', 'Laravel',
      ]
    }
  }
}
</script>
