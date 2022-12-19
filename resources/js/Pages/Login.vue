<script setup>
import { Head, Link } from '@inertiajs/inertia-vue3';
</script>
<template>
    <Head title="Login" />
    <main class="h-screen">
    <!-- =========={ login }==========  -->
    <div id="login-area" class="bg-gray-100 dark:bg-gray-900 dark:bg-opacity-40 flex h-screen items-center py-12 relative">
      <div class="container xl:max-w-6xl mx-auto px-4">
        <div class="flex flex-wrap flex-row -mx-4 justify-center">
          <!-- login form -->
          <div class="max-w-full w-full md:w-2/3 lg:w-1/2 px-6 sm:px-12">
            <div class="relative">
              <div class="p-6 sm:py-8 sm:px-12 rounded-lg bg-white dark:bg-gray-800 shadow-xl">
                <form id="login-form">
                  <h1 class="text-2xl leading-normal mb-6 font-bold text-gray-800 dark:text-gray-300 text-center">Login</h1>
                  <hr class="block w-12 h-0.5 mx-auto my-5 bg-gray-700 border-gray-700">
                  <div class="mb-6">
                    <input name="email" class="w-full leading-5 relative py-2 px-4 rounded text-gray-800 bg-white border border-gray-300 overflow-x-auto focus:outline-none focus:border-gray-400 focus:ring-0 dark:text-gray-300 dark:bg-gray-700 dark:border-gray-700 dark:focus:border-gray-600" placeholder="Email address" value="" aria-label="email" type="email" required>
                  </div>
                  <div class="mb-6">
                    <input class="w-full leading-5 relative py-2 px-4 rounded text-gray-800 bg-white border border-gray-300 overflow-x-auto focus:outline-none focus:border-gray-400 focus:ring-0 dark:text-gray-300 dark:bg-gray-700 dark:border-gray-700 dark:focus:border-gray-600" placeholder="Password" aria-label="password" type="password" value="" required>
                  </div>
                  <div class="mb-6">
                    <input class="form-checkbox h-5 w-5 text-indigo-500 dark:bg-gray-700 border border-gray-300 dark:border-gray-700 rounded focus:outline-none" type="checkbox" value="" id="remember" required>
                    <label class="ml-2" for="remember">
                      Remember me
                    </label>
                  </div>
                  <div class="grid">
                    <Link :href="route('dashboard')" type="submit" class="py-2 px-4 inline-block text-center rounded leading-normal text-gray-100 bg-indigo-500 border border-indigo-500 hover:text-white hover:bg-indigo-600 hover:ring-0 hover:border-indigo-600 focus:bg-indigo-600 focus:border-indigo-600 focus:outline-none focus:ring-0">
                    <!-- <i class="fas fa-sign-in"></i> -->
                      <svg xmlns="http://www.w3.org/2000/svg" fill="currentColor" class="inline-block w-4 h-4 mr-2 bi bi-box-arrow-in-right" viewBox="0 0 16 16">
                        <path fill-rule="evenodd" d="M6 3.5a.5.5 0 0 1 .5-.5h8a.5.5 0 0 1 .5.5v9a.5.5 0 0 1-.5.5h-8a.5.5 0 0 1-.5-.5v-2a.5.5 0 0 0-1 0v2A1.5 1.5 0 0 0 6.5 14h8a1.5 1.5 0 0 0 1.5-1.5v-9A1.5 1.5 0 0 0 14.5 2h-8A1.5 1.5 0 0 0 5 3.5v2a.5.5 0 0 0 1 0v-2z"></path>
                        <path fill-rule="evenodd" d="M11.854 8.354a.5.5 0 0 0 0-.708l-3-3a.5.5 0 1 0-.708.708L10.293 7.5H1.5a.5.5 0 0 0 0 1h8.793l-2.147 2.146a.5.5 0 0 0 .708.708l3-3z"></path>
                      </svg>Login
                    </Link>
                  </div>
                </form>

              </div>
            </div>
          </div>
        </div>
      </div>
    </div><!-- End login -->
  </main>
</template>
