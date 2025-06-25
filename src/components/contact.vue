<template>
  <div class="min-h-screen py-20 bg-gradient-to-br from-slate-50 via-blue-50 to-indigo-50">
    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8">
      <!-- Header Section -->
      <div class="text-center mb-20">
        <div class="inline-block p-3 bg-gradient-to-r from-blue-100 to-indigo-100 rounded-full mb-6">
          <svg class="w-8 h-8 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z"/>
          </svg>
        </div>
        <h1 class="text-5xl md:text-6xl font-bold bg-gradient-to-r from-gray-900 via-blue-900 to-indigo-900 bg-clip-text text-transparent mb-6">
          Get In Touch
        </h1>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto leading-relaxed">
          Ready to bring your ideas to life? Let's collaborate and create something amazing together. 
          I'm always excited to work on new projects and challenges.
        </p>
        <div class="mt-8 flex justify-center">
          <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-full"></div>
        </div>
      </div>

      <div class="grid lg:grid-cols-5 gap-12">
        <!-- Contact Info -->
        <div class="lg:col-span-2 space-y-8">
          <div class="bg-white rounded-2xl p-8 shadow-xl border border-gray-100">
            <h2 class="text-2xl font-bold text-gray-900 mb-8 flex items-center">
              <div class="w-8 h-8 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-lg flex items-center justify-center mr-3">
                <svg class="w-4 h-4 text-white" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z"/>
                  <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z"/>
                </svg>
              </div>
              Contact Information
            </h2>
            
            <div class="space-y-6">
              <div class="group flex items-start gap-4 p-4 rounded-xl hover:bg-blue-50 transition-all duration-300 cursor-pointer">
                <div class="w-12 h-12 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-xl flex items-center justify-center group-hover:scale-110 transition-transform duration-300">
                  <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                  </svg>
                </div>
                <div class="flex-1">
                  <h3 class="font-semibold text-gray-900 mb-1">Email</h3>
                  <p class="text-blue-600 font-medium hover:text-blue-700 transition-colors">
                    nangkhoeum.champhai@student.passerellesnumeriques.org
                  </p>
                  <p class="text-sm text-gray-500 mt-1">I'll respond within 24 hours</p>
                </div>
              </div>

              <div class="group flex items-start gap-4 p-4 rounded-xl hover:bg-green-50 transition-all duration-300 cursor-pointer">
                <div class="w-12 h-12 bg-gradient-to-r from-green-500 to-emerald-500 rounded-xl flex items-center justify-center group-hover:scale-110 transition-transform duration-300">
                  <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                  </svg>
                </div>
                <div class="flex-1">
                  <h3 class="font-semibold text-gray-900 mb-1">Phone</h3>
                  <p class="text-green-600 font-medium hover:text-green-700 transition-colors">
                    +855 12 345 678
                  </p>
                  <p class="text-sm text-gray-500 mt-1">Available Mon-Fri, 9AM-6PM</p>
                </div>
              </div>

              <div class="group flex items-start gap-4 p-4 rounded-xl hover:bg-purple-50 transition-all duration-300 cursor-pointer">
                <div class="w-12 h-12 bg-gradient-to-r from-purple-500 to-pink-500 rounded-xl flex items-center justify-center group-hover:scale-110 transition-transform duration-300">
                  <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                  </svg>
                </div>
                <div class="flex-1">
                  <h3 class="font-semibold text-gray-900 mb-1">Location</h3>
                  <p class="text-purple-600 font-medium">Phnom Penh, Cambodia</p>
                  <p class="text-sm text-gray-500 mt-1">Open to remote work</p>
                </div>
              </div>
            </div>
          </div>

          <!-- Social Links -->
          <div class="bg-white rounded-2xl p-8 shadow-xl border border-gray-100">
            <h3 class="text-xl font-bold text-gray-900 mb-6 flex items-center">
              <div class="w-6 h-6 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-lg flex items-center justify-center mr-3">
                <svg class="w-3 h-3 text-white" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z" clip-rule="evenodd"/>
                </svg>
              </div>
              Connect With Me
            </h3>
            <div class="grid grid-cols-3 gap-4">
              <button class="group relative overflow-hidden bg-gradient-to-r from-gray-800 to-gray-900 rounded-xl p-4 hover:from-gray-700 hover:to-gray-800 transition-all duration-300 transform hover:scale-105">
                <div class="absolute inset-0 bg-gradient-to-r from-blue-500 to-indigo-500 opacity-0 group-hover:opacity-20 transition-opacity duration-300"></div>
                <svg class="h-6 w-6 text-white mx-auto relative z-10" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd" d="M10 0C4.477 0 0 4.484 0 10.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0110 4.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.942.359.31.678.921.678 1.856 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0020 10.017C20 4.484 15.522 0 10 0z" clip-rule="evenodd" />
                </svg>
                <span class="text-xs text-white mt-2 block font-medium">GitHub</span>
              </button>
              
              <button class="group relative overflow-hidden bg-gradient-to-r from-blue-600 to-blue-700 rounded-xl p-4 hover:from-blue-500 hover:to-blue-600 transition-all duration-300 transform hover:scale-105">
                <div class="absolute inset-0 bg-white opacity-0 group-hover:opacity-20 transition-opacity duration-300"></div>
                <svg class="h-6 w-6 text-white mx-auto relative z-10" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M16.338 16.338H13.67V12.16c0-.995-.017-2.277-1.387-2.277-1.39 0-1.601 1.086-1.601 2.207v4.248H8.014v-8.59h2.559v1.174h.037c.356-.675 1.227-1.387 2.526-1.387 2.703 0 3.203 1.778 3.203 4.092v4.711zM5.005 6.575a1.548 1.548 0 11-.003-3.096 1.548 1.548 0 01.003 3.096zm-1.337 9.763H6.34v-8.59H3.667v8.59zM17.668 1H2.328C1.595 1 1 1.581 1 2.298v15.403C1 18.418 1.595 19 2.328 19h15.34c.734 0 1.332-.582 1.332-1.299V2.298C19 1.581 18.402 1 17.668 1z"/>
                </svg>
                <span class="text-xs text-white mt-2 block font-medium">LinkedIn</span>
              </button>
              
              <button class="group relative overflow-hidden bg-gradient-to-r from-blue-400 to-blue-500 rounded-xl p-4 hover:from-blue-300 hover:to-blue-400 transition-all duration-300 transform hover:scale-105">
                <div class="absolute inset-0 bg-white opacity-0 group-hover:opacity-20 transition-opacity duration-300"></div>
                <svg class="h-6 w-6 text-white mx-auto relative z-10" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M6.29 18.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0020 3.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.073 4.073 0 01.8 7.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 010 16.407a11.616 11.616 0 006.29 1.84"/>
                </svg>
                <span class="text-xs text-white mt-2 block font-medium">Twitter</span>
              </button>
            </div>
          </div>

          <!-- Quick Stats -->
          <div class="bg-gradient-to-r from-blue-600 to-indigo-600 rounded-2xl p-8 text-white">
            <h3 class="text-xl font-bold mb-6">Let's Create Together</h3>
            <div class="grid grid-cols-2 gap-4">
              <div class="text-center">
                <div class="text-2xl font-bold">24h</div>
                <div class="text-blue-100 text-sm">Response Time</div>
              </div>
              <div class="text-center">
                <div class="text-2xl font-bold">4+</div>
                <div class="text-blue-100 text-sm">Projects Done</div>
              </div>
            </div>
          </div>
        </div>

        <!-- Contact Form -->
        <div class="lg:col-span-3">
          <div class="bg-white rounded-2xl p-8 shadow-xl border border-gray-100">
            <div class="mb-8">
              <h2 class="text-2xl font-bold text-gray-900 mb-2">Send Me a Message</h2>
              <p class="text-gray-600">Fill out the form below and I'll get back to you as soon as possible.</p>
            </div>

            <form @submit.prevent="submitForm" class="space-y-6">
              <div class="grid md:grid-cols-2 gap-6">
                <div class="group">
                  <label for="name" class="block text-sm font-semibold text-gray-700 mb-2">
                    Full Name *
                  </label>
                  <div class="relative">
                    <input
                      id="name"
                      v-model="form.name"
                      type="text"
                      required
                      class="w-full px-4 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300"
                      placeholder="Enter your full name"
                    />
                    <div class="absolute inset-y-0 right-0 flex items-center pr-4">
                      <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z"/>
                      </svg>
                    </div>
                  </div>
                </div>

                <div class="group">
                  <label for="email" class="block text-sm font-semibold text-gray-700 mb-2">
                    Email Address *
                  </label>
                  <div class="relative">
                    <input
                      id="email"
                      v-model="form.email"
                      type="email"
                      required
                      class="w-full px-4 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300"
                      placeholder="your.email@example.com"
                    />
                    <div class="absolute inset-y-0 right-0 flex items-center pr-4">
                      <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z"/>
                      </svg>
                    </div>
                  </div>
                </div>
              </div>

              <div class="group">
                <label for="subject" class="block text-sm font-semibold text-gray-700 mb-2">
                  Subject *
                </label>
                <select
                  id="subject"
                  v-model="form.subject"
                  required
                  class="w-full px-4 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300"
                >
                  <option value="">Select a subject</option>
                  <option value="web-development">Web Development Project</option>
                  <option value="collaboration">Collaboration Opportunity</option>
                  <option value="freelance">Freelance Work</option>
                  <option value="consultation">Technical Consultation</option>
                  <option value="other">Other</option>
                </select>
              </div>

              <div class="group">
                <label for="message" class="block text-sm font-semibold text-gray-700 mb-2">
                  Message *
                </label>
                <textarea
                  id="message"
                  v-model="form.message"
                  rows="6"
                  required
                  class="w-full px-4 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300 resize-none"
                  placeholder="Tell me about your project, ideas, or how we can work together..."
                ></textarea>
                <div class="text-right mt-2">
                  <span class="text-sm text-gray-500">{{ form.message.length }}/500</span>
                </div>
              </div>

              <div class="flex items-center space-x-3">
                <input
                  id="agree"
                  v-model="form.agree"
                  type="checkbox"
                  required
                  class="w-4 h-4 text-blue-600 border-2 border-gray-300 rounded focus:ring-blue-500"
                />
                <label for="agree" class="text-sm text-gray-600">
                  I agree to the <a href="#" class="text-blue-600 hover:text-blue-700 font-medium">privacy policy</a> and <a href="#" class="text-blue-600 hover:text-blue-700 font-medium">terms of service</a>
                </label>
              </div>

              <button
                type="submit"
                :disabled="isSubmitting"
                class="w-full bg-gradient-to-r from-blue-600 to-indigo-600 text-white py-4 px-8 rounded-xl font-semibold hover:from-blue-700 hover:to-indigo-700 focus:ring-4 focus:ring-blue-100 transition-all duration-300 transform hover:scale-[1.02] disabled:opacity-50 disabled:cursor-not-allowed flex items-center justify-center space-x-2"
              >
                <span v-if="!isSubmitting">Send Message</span>
                <span v-else>Sending...</span>
                <svg v-if="!isSubmitting" class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8"/>
                </svg>
                <svg v-else class="animate-spin w-5 h-5" fill="none" viewBox="0 0 24 24">
                  <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                  <path class="opacity-75" fill="currentColor" d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z"></path>
                </svg>
              </button>
            </form>
          </div>
        </div>
      </div>

      <!-- Success Message -->
      <div v-if="showSuccess" class="fixed inset-0 bg-black bg-opacity-50 flex items-center justify-center z-50">
        <div class="bg-white rounded-2xl p-8 max-w-md mx-4 text-center">
          <div class="w-16 h-16 bg-green-100 rounded-full flex items-center justify-center mx-auto mb-4">
            <svg class="w-8 h-8 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7"/>
            </svg>
          </div>
          <h3 class="text-xl font-bold text-gray-900 mb-2">Message Sent!</h3>
          <p class="text-gray-600 mb-6">Thank you for reaching out. I'll get back to you within 24 hours.</p>
          <button @click="showSuccess = false" class="bg-blue-600 text-white px-6 py-2 rounded-lg hover:bg-blue-700 transition-colors">
            Close
          </button>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'Contact',
  data() {
    return {
      isSubmitting: false,
      showSuccess: false,
      form: {
        name: '',
        email: '',
        subject: '',
        message: '',
        agree: false
      }
    }
  },
  methods: {
    async submitForm() {
      this.isSubmitting = true
      
      // Simulate form submission
      await new Promise(resolve => setTimeout(resolve, 2000))
      
      this.isSubmitting = false
      this.showSuccess = true
      
      // Reset form
      this.form = {
        name: '',
        email: '',
        subject: '',
        message: '',
        agree: false
      }
    }
  }
}
</script>

<style scoped>
@keyframes pulse {
  0%, 100% { opacity: 1; }
  50% { opacity: 0.5; }
}

.animate-pulse {
  animation: pulse 2s cubic-bezier(0.4, 0, 0.6, 1) infinite;
}
</style>
