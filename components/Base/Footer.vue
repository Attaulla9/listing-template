<template>
  <section class="bg-gray-100 dark:bg-gray-800">
    <footer
      class="
        container
        mx-auto
        grid grid-cols-1
        lg:grid-cols-4
        xl:grid-cols-4
        gap-6
        py-8
        px-4
        lg:px-0
        xl:px-0
      "
    >
      <div class="flex items-center">
        <div class="space-y-4">
          <div class="flex items-center space-x-3">
            <BaseLogo class="h-10 w-10" />
            <p class="font-bold text-2xl">JamstackMakers</p>
          </div>
          <p class="text-gray-500 dark:text-gray-300 text-sm">
            Jamstack projects from the makers community.
          </p>
        </div>
      </div>
      <div></div>
      <div>
        <p class="font-semibold text-gray-800 mb-2">Links</p>
        <ul class="space-y-1">
          <li><nuxt-link to="/">About</nuxt-link></li>
          <li><nuxt-link to="/">Projects</nuxt-link></li>
          <li><nuxt-link to="/">Community</nuxt-link></li>
          <li><nuxt-link to="/">Articles</nuxt-link></li>
        </ul>
      </div>
      <div>
        <p class="font-semibold text-gray-800 mb-2">Legal</p>
        <ul class="space-y-1">
          <li>
            <nuxt-link to="/terms-and-conditions"
              >Terms &amp; Conditions</nuxt-link
            >
          </li>
        </ul>
      </div>
    </footer>
    <div class="bg-gray-200 dark:bg-gray-700">
      <div
        class="container mx-auto py-4 px-5 flex flex-wrap flex-col sm:flex-row"
      >
        <p
          class="
            text-gray-500
            dark:text-gray-300
            text-sm text-center
            sm:text-left
          "
        >
          © {{ currentYear }} Jamstack Makers —
          <a
            href="https://twitter.com"
            rel="noopener noreferrer"
            class="text-gray-600 dark:text-gray-400 ml-1"
            target="_blank"
            >@jamstackmakers</a
          >
        </p>
        <span
          class="
            inline-flex
            sm:ml-auto
            sm:mt-0
            mt-2
            justify-center
            sm:justify-start
          "
        >
          <a class="text-gray-500 dark:text-gray-300">
            <svg
              fill="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="w-5 h-5"
              viewBox="0 0 24 24"
            >
              <path
                d="M18 2h-3a5 5 0 00-5 5v3H7v4h3v8h4v-8h3l1-4h-4V7a1 1 0 011-1h3z"
              ></path>
            </svg>
          </a>
          <a class="ml-3 text-gray-500 dark:text-gray-300">
            <svg
              fill="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="w-5 h-5"
              viewBox="0 0 24 24"
            >
              <path
                d="M23 3a10.9 10.9 0 01-3.14 1.53 4.48 4.48 0 00-7.86 3v1A10.66 10.66 0 013 4s-4 9 5 13a11.64 11.64 0 01-7 2c9 5 20 0 20-11.5a4.5 4.5 0 00-.08-.83A7.72 7.72 0 0023 3z"
              ></path>
            </svg>
          </a>
          <a class="ml-3 text-gray-500 dark:text-gray-300">
            <svg
              fill="none"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              class="w-5 h-5"
              viewBox="0 0 24 24"
            >
              <rect width="20" height="20" x="2" y="2" rx="5" ry="5"></rect>
              <path
                d="M16 11.37A4 4 0 1112.63 8 4 4 0 0116 11.37zm1.5-4.87h.01"
              ></path>
            </svg>
          </a>
          <a class="ml-3 text-gray-500 dark:text-gray-300">
            <svg
              fill="currentColor"
              stroke="currentColor"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="0"
              class="w-5 h-5"
              viewBox="0 0 24 24"
            >
              <path
                stroke="none"
                d="M16 8a6 6 0 016 6v7h-4v-7a2 2 0 00-2-2 2 2 0 00-2 2v7h-4v-7a6 6 0 016-6zM2 9h4v12H2z"
              ></path>
              <circle cx="4" cy="4" r="2" stroke="none"></circle>
            </svg>
          </a>
        </span>
      </div>
    </div>
  </section>
</template>

<script>
export default {
  computed: {
    currentYear() {
      let dd = new Date();
      return dd.getFullYear();
    },
  },
};
</script>