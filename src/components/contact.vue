<template>
  <div class="min-h-screen py-20 bg-gradient-to-br from-slate-50 via-blue-50 to-indigo-50 relative overflow-hidden">
    <!-- Professional floating elements -->
    <div class="absolute inset-0 overflow-hidden pointer-events-none">
      <div class="absolute top-20 left-10 w-72 h-72 bg-blue-200/20 rounded-full blur-3xl animate-pulse"></div>
      <div class="absolute bottom-20 right-10 w-96 h-96 bg-indigo-200/20 rounded-full blur-3xl animate-pulse"
        style="animation-delay: 2s;"></div>
      <div class="absolute top-1/2 left-1/3 w-64 h-64 bg-purple-200/20 rounded-full blur-3xl animate-pulse"
        style="animation-delay: 4s;"></div>
    </div>

    <div class="max-w-6xl mx-auto px-4 sm:px-6 lg:px-8 relative z-10">
      <!-- Enhanced Header Section -->
      <div class="text-center mb-20">
        <div
          class="inline-block p-4 bg-gradient-to-r from-blue-100 to-indigo-100 rounded-full mb-6 shadow-lg animate-bounce-slow">
          <svg class="w-10 h-10 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
            <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
              d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z" />
          </svg>
        </div>
        <h1
          class="text-5xl md:text-7xl font-bold bg-gradient-to-r from-gray-900 via-blue-900 to-indigo-900 bg-clip-text text-transparent mb-6 animate-fade-in-up">
          Get In Touch
        </h1>
        <p class="text-xl text-gray-600 max-w-3xl mx-auto leading-relaxed mb-8">
          Ready to bring your ideas to life? Let's collaborate and create something amazing together.
          I'm always excited to work on new projects and challenges.
        </p>
        <div class="flex justify-center items-center gap-4 mb-8">
          <div class="w-24 h-1 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-full animate-pulse"></div>
          <div class="w-3 h-3 bg-blue-500 rounded-full animate-ping"></div>
          <div class="w-24 h-1 bg-gradient-to-r from-indigo-500 to-purple-500 rounded-full animate-pulse"></div>
        </div>
        <!-- Professional badges -->
        <div class="flex justify-center gap-4 flex-wrap">
          <span
            class="inline-flex items-center px-4 py-2 rounded-full text-sm font-medium bg-blue-100 text-blue-800 shadow-sm">
            <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
            Quick Response
          </span>
          <span
            class="inline-flex items-center px-4 py-2 rounded-full text-sm font-medium bg-green-100 text-green-800 shadow-sm">
            <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M9 12l2 2 4-4m6 2a9 9 0 11-18 0 9 9 0 0118 0z" />
            </svg>
            Professional
          </span>
          <span
            class="inline-flex items-center px-4 py-2 rounded-full text-sm font-medium bg-purple-100 text-purple-800 shadow-sm">
            <svg class="w-4 h-4 mr-2" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M13 10V3L4 14h7v7l9-11h-7z" />
            </svg>
            Fast Delivery
          </span>
        </div>
      </div>

      <div class="grid lg:grid-cols-5 gap-12">
        <!-- Enhanced Contact Info -->
        <div class="lg:col-span-2 space-y-8">
          <div
            class="bg-white/90 backdrop-blur-sm rounded-2xl p-8 shadow-2xl border border-gray-100/50 hover:shadow-3xl transition-all duration-500">
            <h2 class="text-2xl font-bold text-gray-900 mb-8 flex items-center">
              <div
                class="w-8 h-8 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-lg flex items-center justify-center mr-3 shadow-lg">
                <svg class="w-4 h-4 text-white" fill="currentColor" viewBox="0 0 20 20">
                  <path d="M2.003 5.884L10 9.882l7.997-3.998A2 2 0 0016 4H4a2 2 0 00-1.997 1.884z" />
                  <path d="M18 8.118l-8 4-8-4V14a2 2 0 002 2h12a2 2 0 002-2V8.118z" />
                </svg>
              </div>
              Contact Information
            </h2>

            <div class="space-y-6">
              <div
                class="group flex items-start gap-4 p-5 rounded-xl hover:bg-blue-50 transition-all duration-300 cursor-pointer border border-transparent hover:border-blue-200 hover:shadow-lg">
                <div
                  class="w-14 h-14 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-xl flex items-center justify-center group-hover:scale-110 transition-transform duration-300 shadow-lg">
                  <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                  </svg>
                </div>
                <div class="flex-1">
                  <h3 class="font-semibold text-gray-900 mb-1 text-lg">Email</h3>
                  <p class="text-blue-600 font-medium hover:text-blue-700 transition-colors break-all">
                    nangkhoeum.champhai@student.passerellesnumeriques.org
                  </p>
                  <p class="text-sm text-gray-500 mt-2 flex items-center">
                    <svg class="w-4 h-4 mr-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                    I'll respond within 24 hours
                  </p>
                </div>
              </div>

              <div
                class="group flex items-start gap-4 p-5 rounded-xl hover:bg-green-50 transition-all duration-300 cursor-pointer border border-transparent hover:border-green-200 hover:shadow-lg">
                <div
                  class="w-14 h-14 bg-gradient-to-r from-green-500 to-emerald-500 rounded-xl flex items-center justify-center group-hover:scale-110 transition-transform duration-300 shadow-lg">
                  <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M3 5a2 2 0 012-2h3.28a1 1 0 01.948.684l1.498 4.493a1 1 0 01-.502 1.21l-2.257 1.13a11.042 11.042 0 005.516 5.516l1.13-2.257a1 1 0 011.21-.502l4.493 1.498a1 1 0 01.684.949V19a2 2 0 01-2 2h-1C9.716 21 3 14.284 3 6V5z" />
                  </svg>
                </div>
                <div class="flex-1">
                  <h3 class="font-semibold text-gray-900 mb-1 text-lg">Phone</h3>
                  <p class="text-green-600 font-medium hover:text-green-700 transition-colors">
                    +855 97 85 44 641
                  </p>
                  <p class="text-sm text-gray-500 mt-2 flex items-center">
                    <svg class="w-4 h-4 mr-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M8 7V3a2 2 0 012-2h4a2 2 0 012 2v4m-6 9a2 2 0 11-4 0 2 2 0 014 0z" />
                    </svg>
                    Available Mon-Fri, 9AM-6PM
                  </p>
                </div>
              </div>

              <div
                class="group flex items-start gap-4 p-5 rounded-xl hover:bg-purple-50 transition-all duration-300 cursor-pointer border border-transparent hover:border-purple-200 hover:shadow-lg">
                <div
                  class="w-14 h-14 bg-gradient-to-r from-purple-500 to-pink-500 rounded-xl flex items-center justify-center group-hover:scale-110 transition-transform duration-300 shadow-lg">
                  <svg class="h-6 w-6 text-white" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M17.657 16.657L13.414 20.9a1.998 1.998 0 01-2.827 0l-4.244-4.243a8 8 0 1111.314 0z" />
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M15 11a3 3 0 11-6 0 3 3 0 016 0z" />
                  </svg>
                </div>
                <div class="flex-1">
                  <h3 class="font-semibold text-gray-900 mb-1 text-lg">Location</h3>
                  <p class="text-purple-600 font-medium">Phnom Penh, Cambodia</p>
                  <p class="text-sm text-gray-500 mt-2 flex items-center">
                    <svg class="w-4 h-4 mr-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M21 12a9 9 0 01-9 9m9-9a9 9 0 00-9-9m9 9H3m9 9v-9m0-9v9" />
                    </svg>
                    Open to remote work
                  </p>
                </div>
              </div>
            </div>
          </div>

          <!-- Enhanced Social Links -->
          <div
            class="bg-white/90 backdrop-blur-sm rounded-2xl p-8 shadow-2xl border border-gray-100/50 hover:shadow-3xl transition-all duration-500">
            <h3 class="text-xl font-bold text-gray-900 mb-6 flex items-center">
              <div
                class="w-6 h-6 bg-gradient-to-r from-blue-500 to-indigo-500 rounded-lg flex items-center justify-center mr-3 shadow-lg">
                <svg class="w-3 h-3 text-white" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd"
                    d="M3 5a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 10a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1zM3 15a1 1 0 011-1h12a1 1 0 110 2H4a1 1 0 01-1-1z"
                    clip-rule="evenodd" />
                </svg>
              </div>
              Connect With Me
            </h3>
            <div class="grid grid-cols-3 gap-4">
              <button
                class="group relative overflow-hidden bg-gradient-to-r from-gray-800 to-gray-900 rounded-xl p-5 hover:from-gray-700 hover:to-gray-800 transition-all duration-300 transform hover:scale-105 hover:shadow-xl">
                <div
                  class="absolute inset-0 bg-gradient-to-r from-blue-500 to-indigo-500 opacity-0 group-hover:opacity-20 transition-opacity duration-300">
                </div>
                <svg class="h-7 w-7 text-white mx-auto relative z-10 mb-2" fill="currentColor" viewBox="0 0 20 20">
                  <path fill-rule="evenodd"
                    d="M10 0C4.477 0 0 4.484 0 10.017c0 4.425 2.865 8.18 6.839 9.504.5.092.682-.217.682-.483 0-.237-.008-.868-.013-1.703-2.782.605-3.369-1.343-3.369-1.343-.454-1.158-1.11-1.466-1.11-1.466-.908-.62.069-.608.069-.608 1.003.07 1.531 1.032 1.531 1.032.892 1.53 2.341 1.088 2.91.832.092-.647.35-1.088.636-1.338-2.22-.253-4.555-1.113-4.555-4.951 0-1.093.39-1.988 1.029-2.688-.103-.253-.446-1.272.098-2.65 0 0 .84-.27 2.75 1.026A9.564 9.564 0 0110 4.844c.85.004 1.705.115 2.504.337 1.909-1.296 2.747-1.027 2.747-1.027.546 1.379.203 2.398.1 2.651.64.7 1.028 1.595 1.028 2.688 0 3.848-2.339 4.695-4.566 4.942.359.31.678.921.678 1.856 0 1.338-.012 2.419-.012 2.747 0 .268.18.58.688.482A10.019 10.019 0 0020 10.017C20 4.484 15.522 0 10 0z"
                    clip-rule="evenodd" />
                </svg>
                <span class="text-sm text-white font-medium relative z-10">GitHub</span>
              </button>

              <button
                class="group relative overflow-hidden bg-gradient-to-r from-blue-600 to-blue-700 rounded-xl p-5 hover:from-blue-500 hover:to-blue-600 transition-all duration-300 transform hover:scale-105 hover:shadow-xl">
                <div class="absolute inset-0 bg-white opacity-0 group-hover:opacity-20 transition-opacity duration-300">
                </div>
                <svg class="h-7 w-7 text-white mx-auto relative z-10 mb-2" fill="currentColor" viewBox="0 0 20 20">
                  <path
                    d="M16.338 16.338H13.67V12.16c0-.995-.017-2.277-1.387-2.277-1.39 0-1.601 1.086-1.601 2.207v4.248H8.014v-8.59h2.559v1.174h.037c.356-.675 1.227-1.387 2.526-1.387 2.703 0 3.203 1.778 3.203 4.092v4.711zM5.005 6.575a1.548 1.548 0 11-.003-3.096 1.548 1.548 0 01.003 3.096zm-1.337 9.763H6.34v-8.59H3.667v8.59zM17.668 1H2.328C1.595 1 1 1.581 1 2.298v15.403C1 18.418 1.595 19 2.328 19h15.34c.734 0 1.332-.582 1.332-1.299V2.298C19 1.581 18.402 1 17.668 1z" />
                </svg>
                <span class="text-sm text-white font-medium relative z-10">LinkedIn</span>
              </button>

              <button
                class="group relative overflow-hidden bg-gradient-to-r from-blue-400 to-blue-500 rounded-xl p-5 hover:from-blue-300 hover:to-blue-400 transition-all duration-300 transform hover:scale-105 hover:shadow-xl">
                <div class="absolute inset-0 bg-white opacity-0 group-hover:opacity-20 transition-opacity duration-300">
                </div>
                <svg class="h-7 w-7 text-white mx-auto relative z-10 mb-2" fill="currentColor" viewBox="0 0 20 20">
                  <path
                    d="M6.29 18.251c7.547 0 11.675-6.253 11.675-11.675 0-.178 0-.355-.012-.53A8.348 8.348 0 0020 3.92a8.19 8.19 0 01-2.357.646 4.118 4.118 0 001.804-2.27 8.224 8.224 0 01-2.605.996 4.107 4.107 0 00-6.993 3.743 11.65 11.65 0 01-8.457-4.287 4.106 4.106 0 001.27 5.477A4.073 4.073 0 01.8 7.713v.052a4.105 4.105 0 003.292 4.022 4.095 4.095 0 01-1.853.07 4.108 4.108 0 003.834 2.85A8.233 8.233 0 010 16.407a11.616 11.616 0 006.29 1.84" />
                </svg>
                <span class="text-sm text-white font-medium relative z-10">Twitter</span>
              </button>
            </div>
          </div>

          <!-- Enhanced Quick Stats -->
          <div
            class="bg-gradient-to-r from-blue-600 via-indigo-600 to-purple-600 rounded-2xl p-8 text-white shadow-2xl relative overflow-hidden">
            <div class="absolute inset-0 bg-gradient-to-r from-blue-400/30 to-purple-400/30 animate-pulse"></div>
            <div class="relative z-10">
              <h3 class="text-xl font-bold mb-6 flex items-center">
                <svg class="w-6 h-6 mr-2 text-pink-300" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
                </svg>
                Let's Create Together
              </h3>
              <div class="grid grid-cols-2 gap-6">
                <div
                  class="text-center p-4 bg-white/10 rounded-xl backdrop-blur-sm border border-white/20 hover:bg-white/20 transition-all duration-300">
                  <div class="text-3xl font-bold mb-1 flex items-center justify-center">
                    24h
                    <svg class="w-6 h-6 ml-2 text-blue-200" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M12 8v4l3 3m6-3a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                  </div>
                  <div class="text-blue-100 text-sm font-medium">Response Time</div>
                </div>
                <div
                  class="text-center p-4 bg-white/10 rounded-xl backdrop-blur-sm border border-white/20 hover:bg-white/20 transition-all duration-300">
                  <div class="text-3xl font-bold mb-1 flex items-center justify-center">
                    4+
                    <svg class="w-6 h-6 ml-2 text-yellow-300" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M11.049 2.927c.3-.921 1.603-.921 1.902 0l1.519 4.674a1 1 0 00.95.69h4.915c.969 0 1.371 1.24.588 1.81l-3.976 2.888a1 1 0 00-.363 1.118l1.518 4.674c.3.922-.755 1.688-1.538 1.118l-3.976-2.888a1 1 0 00-1.176 0l-3.976 2.888c-.783.57-1.838-.197-1.538-1.118l1.518-4.674a1 1 0 00-.363-1.118l-3.976-2.888c-.784-.57-.38-1.81.588-1.81h4.914a1 1 0 00.951-.69l1.519-4.674z" />
                    </svg>
                  </div>
                  <div class="text-blue-100 text-sm font-medium">Projects Done</div>
                </div>
              </div>
            </div>
          </div>
        </div>

        <!-- Enhanced Contact Form -->
        <div class="lg:col-span-3">
          <div
            class="bg-white/90 backdrop-blur-sm rounded-2xl p-8 shadow-2xl border border-gray-100/50 hover:shadow-3xl transition-all duration-500">
            <div class="mb-8">
              <h2 class="text-2xl font-bold text-gray-900 mb-3 flex items-center">
                <svg class="w-7 h-7 mr-3 text-blue-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                  <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                    d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8" />
                </svg>
                Send Me a Message
              </h2>
              <p class="text-gray-600 leading-relaxed">Fill out the form below and I'll get back to you as soon as
                possible with a thoughtful response.</p>
            </div>

            <form @submit.prevent="submitForm" class="space-y-6">
              <div class="grid md:grid-cols-2 gap-6">
                <div class="group">
                  <label for="name" class="block text-sm font-semibold text-gray-700 mb-3 flex items-center">
                    <svg class="w-4 h-4 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
                    </svg>
                    Full Name *
                  </label>
                  <div class="relative">
                    <input id="name" v-model="form.name" type="text" required
                      class="w-full px-5 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300 bg-white/80 backdrop-blur-sm shadow-sm"
                      placeholder="Enter your full name" />
                    <div class="absolute inset-y-0 right-0 flex items-center pr-4">
                      <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                          d="M16 7a4 4 0 11-8 0 4 4 0 018 0zM12 14a7 7 0 00-7 7h14a7 7 0 00-7-7z" />
                      </svg>
                    </div>
                  </div>
                </div>

                <div class="group">
                  <label for="email" class="block text-sm font-semibold text-gray-700 mb-3 flex items-center">
                    <svg class="w-4 h-4 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                    </svg>
                    Email Address *
                  </label>
                  <div class="relative">
                    <input id="email" v-model="form.email" type="email" required
                      class="w-full px-5 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300 bg-white/80 backdrop-blur-sm shadow-sm"
                      placeholder="your email@gmail.com" />
                    <div class="absolute inset-y-0 right-0 flex items-center pr-4">
                      <svg class="w-5 h-5 text-gray-400" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                          d="M3 8l7.89 4.26a2 2 0 002.22 0L21 8M5 19h14a2 2 0 002-2V7a2 2 0 00-2-2H5a2 2 0 00-2 2v10a2 2 0 002 2z" />
                      </svg>
                    </div>
                  </div>
                </div>
              </div>

              <div class="group">
                <label for="subject" class="block text-sm font-semibold text-gray-700 mb-3 flex items-center">
                  <svg class="w-4 h-4 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M7 7h.01M7 3h5c.512 0 1.024.195 1.414.586l7 7a2 2 0 010 2.828l-7 7a2 2 0 01-2.828 0l-7-7A1.994 1.994 0 013 12V7a4 4 0 014-4z" />
                  </svg>
                  Subject *
                </label>
                <select id="subject" v-model="form.subject" required
                  class="w-full px-5 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300 bg-white/80 backdrop-blur-sm shadow-sm">
                  <option value="">Select a subject</option>
                  <option value="web-development">🚀 Web Development Project</option>
                  <option value="collaboration">🤝 Collaboration Opportunity</option>
                  <option value="freelance">💼 Freelance Work</option>
                  <option value="consultation">💡 Technical Consultation</option>
                  <option value="other">📝 Other</option>
                </select>
              </div>

              <div class="group">
                <label for="message" class="block text-sm font-semibold text-gray-700 mb-3 flex items-center">
                  <svg class="w-4 h-4 mr-2 text-gray-500" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M8 12h.01M12 12h.01M16 12h.01M21 12c0 4.418-4.03 8-9 8a9.863 9.863 0 01-4.255-.949L3 20l1.395-3.72C3.512 15.042 3 13.574 3 12c0-4.418 4.03-8 9-8s9 3.582 9 8z" />
                  </svg>
                  Message *
                </label>
                <textarea id="message" v-model="form.message" rows="6" required maxlength="500"
                  class="w-full px-5 py-4 border-2 border-gray-200 rounded-xl focus:ring-4 focus:ring-blue-100 focus:border-blue-500 transition-all duration-300 group-hover:border-gray-300 resize-none bg-white/80 backdrop-blur-sm shadow-sm"
                  placeholder="Tell me about your project, ideas, or how we can work together..."></textarea>
                <div class="flex justify-between items-center mt-3">
                  <div class="text-sm text-gray-500 flex items-center">
                    <svg class="w-4 h-4 mr-1" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                      <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                        d="M13 16h-1v-4h-1m1-4h.01M21 12a9 9 0 11-18 0 9 9 0 0118 0z" />
                    </svg>
                    Be specific about your requirements
                  </div>
                  <span class="text-sm font-medium"
                    :class="form.message.length > 450 ? 'text-red-500' : 'text-gray-500'">
                    {{ form.message.length }}/500
                  </span>
                </div>
              </div>

              <div class="flex items-start space-x-3 p-4 bg-gray-50 rounded-xl border border-gray-200">
                <input id="agree" v-model="form.agree" type="checkbox" required
                  class="w-5 h-5 text-blue-600 border-2 border-gray-300 rounded focus:ring-blue-500 mt-0.5" />
                <label for="agree" class="text-sm text-gray-600 leading-relaxed">
                  I agree to the <a href="#"
                    class="text-blue-600 hover:text-blue-700 font-medium underline decoration-2 underline-offset-2">privacy
                    policy</a> and <a href="#"
                    class="text-blue-600 hover:text-blue-700 font-medium underline decoration-2 underline-offset-2">terms
                    of service</a>. I understand that my information will be handled professionally and securely.
                </label>
              </div>

              <button type="submit" :disabled="isSubmitting"
                class="w-full bg-gradient-to-r from-blue-600 via-indigo-600 to-purple-600 text-white py-5 px-8 rounded-xl font-semibold text-lg hover:from-blue-700 hover:via-indigo-700 hover:to-purple-700 focus:ring-4 focus:ring-blue-100 transition-all duration-300 transform hover:scale-[1.02] disabled:opacity-50 disabled:cursor-not-allowed flex items-center justify-center space-x-3 shadow-xl hover:shadow-2xl">
                <span v-if="!isSubmitting" class="flex items-center space-x-2">
                  <span>Send Message</span>
                  <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
                    <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                      d="M12 19l9 2-9-18-9 18 9-2zm0 0v-8" />
                  </svg>
                </span>
                <span v-else class="flex items-center space-x-2">
                  <svg class="animate-spin w-5 h-5" fill="none" viewBox="0 0 24 24">
                    <circle class="opacity-25" cx="12" cy="12" r="10" stroke="currentColor" stroke-width="4"></circle>
                    <path class="opacity-75" fill="currentColor"
                      d="M4 12a8 8 0 018-8V0C5.373 0 0 5.373 0 12h4zm2 5.291A7.962 7.962 0 014 12H0c0 3.042 1.135 5.824 3 7.938l3-2.647z">
                    </path>
                  </svg>
                  <span>Sending your message...</span>
                </span>
              </button>
            </form>
          </div>
        </div>
      </div>

      <!-- Enhanced Success Message -->
      <div v-if="showSuccess"
        class="fixed inset-0 bg-black/60 backdrop-blur-sm flex items-center justify-center z-50 animate-fade-in">
        <div
          class="bg-white rounded-2xl p-10 max-w-md mx-4 text-center shadow-3xl border border-gray-100 animate-scale-in">
          <div
            class="w-20 h-20 bg-gradient-to-r from-green-100 to-emerald-100 rounded-full flex items-center justify-center mx-auto mb-6 animate-bounce">
            <svg class="w-10 h-10 text-green-600" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
            </svg>
          </div>
          <h3 class="text-2xl font-bold text-gray-900 mb-3">Message Sent Successfully!</h3>
          <p class="text-gray-600 mb-8 leading-relaxed">Thank you for reaching out. I'll get back to you within 24 hours
            with a thoughtful and detailed response.</p>
          <button @click="showSuccess = false"
            class="bg-gradient-to-r from-blue-600 to-indigo-600 text-white px-8 py-3 rounded-xl hover:from-blue-700 hover:to-indigo-700 transition-all duration-300 font-semibold shadow-lg hover:shadow-xl transform hover:scale-105 flex items-center justify-center mx-auto space-x-2">
            <svg class="w-5 h-5" fill="none" stroke="currentColor" viewBox="0 0 24 24">
              <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2"
                d="M4.318 6.318a4.5 4.5 0 000 6.364L12 20.364l7.682-7.682a4.5 4.5 0 00-6.364-6.364L12 7.636l-1.318-1.318a4.5 4.5 0 00-6.364 0z" />
            </svg>
            <span>Close</span>
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

      // Simulate form submission with more realistic timing
      await new Promise(resolve => setTimeout(resolve, 2500))

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
/* Enhanced animations */
@keyframes fade-in-up {
  from {
    opacity: 0;
    transform: translateY(30px);
  }

  to {
    opacity: 1;
    transform: translateY(0);
  }
}

@keyframes bounce-slow {

  0%,
  100% {
    transform: translateY(-5%);
    animation-timing-function: cubic-bezier(0.8, 0, 1, 1);
  }

  50% {
    transform: translateY(0);
    animation-timing-function: cubic-bezier(0, 0, 0.2, 1);
  }
}

@keyframes fade-in {
  from {
    opacity: 0;
  }

  to {
    opacity: 1;
  }
}

@keyframes scale-in {
  from {
    opacity: 0;
    transform: scale(0.95);
  }

  to {
    opacity: 1;
    transform: scale(1);
  }
}

.animate-fade-in-up {
  animation: fade-in-up 0.8s ease-out;
}

.animate-bounce-slow {
  animation: bounce-slow 3s infinite;
}

.animate-fade-in {
  animation: fade-in 0.3s ease-out;
}

.animate-scale-in {
  animation: scale-in 0.3s ease-out;
}

/* Enhanced shadows */
.shadow-3xl {
  box-shadow: 0 35px 60px -12px rgba(0, 0, 0, 0.25);
}

/* Smooth transitions for all interactive elements */
* {
  transition-property: all;
  transition-timing-function: cubic-bezier(0.4, 0, 0.2, 1);
}

/* Enhanced focus states */
input:focus,
textarea:focus,
select:focus {
  outline: none;
  box-shadow: 0 0 0 4px rgba(59, 130, 246, 0.1);
}

/* Professional hover effects */
.group:hover .group-hover\:scale-110 {
  transform: scale(1.1);
}

/* Enhanced backdrop blur */
.backdrop-blur-sm {
  backdrop-filter: blur(8px);
}
</style>