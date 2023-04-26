<template>
  <nav class="w-full top-0 p-6 bg-white">
    <div class="flex items-center justify-between">
      <div>
        <nuxt-link to="/" class="flex items-center">
          <img src="~/assets/MBL_Logo.png" class="h-8 mr-3" alt="MBL Engineering Logo">
          <span class="self-center text-2xl font-semibold whitespace-nowrap">MBL Engineering</span>
        </nuxt-link>
      </div>

      <div class="md:hidden">
        <button @click="drawer">
          <svg
            class="h-8 w-8 fill-current text-black"
            fill="none"
            stroke-linecap="round"
            stroke-linejoin="round"
            stroke-width="2"
            viewBox="0 0 24 24"
            stroke="currentColor"
          >
            <path d="M4 6h16M4 12h16M4 18h16" />
          </svg>
        </button>
      </div>

      <div class="hidden md:block">
        <ul class="flex space-x-8 text-sm font-sans">
          <li>
            <nuxt-link to="/">
              Home
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/#about">
              About
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/#product">
              Products
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/#contact">
              Contact
            </nuxt-link>
          </li>
        </ul>
      </div>

      <transition
        enter-class="opacity-0"
        enter-active-class="ease-out transition-medium"
        enter-to-class="opacity-100"
        leave-class="opacity-100"
        leave-active-class="ease-out transition-medium"
        leave-to-class="opacity-0"
      >
        <div v-show="isOpen" class="z-10 fixed inset-0 transition-opacity" @keydown.esc="isOpen = false">
          <div class="absolute inset-0 bg-black opacity-50" tabindex="0" @click="isOpen = false" />
        </div>
      </transition>

      <aside class="p-5 transform top-0 left-0 w-64 bg-white fixed h-full overflow-auto ease-in-out transition-all duration-300 z-30" :class="isOpen ? 'translate-x-0' : '-translate-x-full'">
        <div class="close">
          <button class="absolute top-0 right-0 mt-4 mr-4" @click=" isOpen = false">
            <svg
              class="w-6 h-6"
              fill="none"
              stroke-linecap="round"
              stroke-linejoin="round"
              stroke-width="2"
              viewBox="0 0 24 24"
              stroke="currentColor"
            >
              <path d="M6 18L18 6M6 6l12 12" />
            </svg>
          </button>
        </div>

        <span class="flex w-full items-center p-4 border-b" @click="isOpen = false">
          <div>
            <nuxt-link to="#" class="flex items-center">
              <img src="~/assets/MBL_Logo.png" class="h-8 mr-3" alt="MBL Engineering Logo">
              <span class="self-center text-xl font-semibold whitespace-nowrap">MBL Engineering</span>
            </nuxt-link>
          </div>
        </span>

        <ul class="divide-y font-sans">
          <li>
            <nuxt-link to="/">
              <div class="my-4 inline-block" @click="isOpen = false">
                Home
              </div>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/#about">
              <div class="my-4 inline-block" @click="isOpen = false">
                About
              </div>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/#product">
              <div class="my-4 inline-block" @click="isOpen = false">
                Product
              </div>
            </nuxt-link>
          </li>
          <li>
            <nuxt-link to="/#contact">
              <div class="my-4 inline-block" @click="isOpen = false">
                Contact
              </div>
            </nuxt-link>
          </li>
        </ul>
      </aside>
    </div>
  </nav>
</template>

<script>

export default {
  name: 'HeaderNBL',
  data () {
    return {
      isOpen: false
    }
  },
  watch: {
    isOpen: {
      immediate: true,
      handler (isOpen) {
        if (process.client) {
          if (isOpen) { document.body.style.setProperty('overflow', 'hidden') } else { document.body.style.removeProperty('overflow') }
        }
      }
    }
  },
  mounted () {
    document.addEventListener('keydown', (e) => {
      if (e.keyCode === 27 && this.isOpen) { this.isOpen = false }
    })
  },
  methods: {
    drawer () {
      this.isOpen = !this.isOpen
    }
  }
}
</script>
