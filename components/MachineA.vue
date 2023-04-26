<template>
  <div id="machine" class="bg-white py-24 sm:py-32">
    <div class="mx-auto max-w-7xl px-6 lg:px-8">
      <div class="mx-auto max-w-2xl lg:text-center">
        <p class="mt-2 text-3xl font-bold tracking-tight text-[var(--app-color)] sm:text-4xl uppercase">
          Machine | เครื่องจักร
        </p>
      </div>
      <div class="mx-auto mt-16 max-w-2xl sm:mt-20 lg:mt-24 lg:max-w-4xl">
        <div class="grid max-w-xl grid-cols-1 gap-x-8 gap-y-10 lg:max-w-none lg:grid-cols-2 lg:gap-y-16">
          <div id="machine-01" class="pl-16 hover:underline hover:decoration-indigo-500 cursor-pointer">
            <nuxt-link to="/contents/machine-01">
              <div class="text-base font-semibold leading-7 text-gray-900 ">
                3D Measurement FARO
              </div>
              <div class="mt-2 text-base leading-7 text-gray-600">
                <img src="~/assets/DSC_06.jpg" alt="machine-01" class="rounded w-80 ring-offset-2 hover:ring">
              </div>
            </nuxt-link>
          </div>
          <div id="machine-02" class="relative pl-16 hover:underline hover:decoration-indigo-500 cursor-pointer">
            <nuxt-link to="/contents/machine-02">
              <div class="text-base font-semibold leading-7 text-gray-900">
                Laser Cutting Machine
              </div>
              <div class="mt-2 text-base leading-7 text-gray-600">
                <img src="~/assets/DSC_047.jpg" alt="machine-02" class="rounded w-80 ring-offset-2 hover:ring">
              </div>
            </nuxt-link>
          </div>
          <div id="machine-03" class="relative pl-16 hover:underline hover:decoration-indigo-500 cursor-pointer">
            <nuxt-link to="/contents/machine-03">
              <div class="text-base font-semibold leading-7 text-gray-900">
                Robot Welding
              </div>
              <div class="mt-2 text-base leading-7 text-gray-600">
                <img src="~/assets/DSC_042.jpg" alt="machine-03" class="rounded w-80 ring-offset-2 hover:ring">
              </div>
            </nuxt-link>
          </div>
          <div id="machine-04" class="relative pl-16 hover:underline hover:decoration-indigo-500 cursor-pointer">
            <nuxt-link to="/contents/machine-04">
              <div class="text-base font-semibold leading-7 text-gray-900">
                Hydraulic Press Brake Machine
              </div>
              <div class="mt-2 text-base leading-7 text-gray-600">
                <img src="~/assets/DSC_052.jpg" alt="machine-04" class="rounded w-80 ring-offset-2 hover:ring">
              </div>
            </nuxt-link>
          </div>
          <div id="machine-05" class="relative pl-16 hover:underline hover:decoration-indigo-500 cursor-pointer">
            <nuxt-link to="/contents/machine-05">
              <div class="text-base font-semibold leading-7 text-gray-900">
                CNC Milling
              </div>
              <div class="mt-2 text-base leading-7 text-gray-600">
                <img src="~/assets/DSC_027.jpg" alt="machine-05" class="rounded w-80 ring-offset-2 hover:ring">
              </div>
            </nuxt-link>
          </div>
          <div id="machine-06" class="relative pl-16 hover:underline hover:decoration-indigo-500 cursor-pointer">
            <nuxt-link to="/contents/machine-06">
              <div class="text-base font-semibold leading-7 text-gray-900">
                JIG FIXTRUE
              </div>
              <div class="mt-2 text-base leading-7 text-gray-600">
                <img src="~/assets/DSC_039.jpg" alt="machine-06" class="rounded w-80 ring-offset-2 hover:ring">
              </div>
            </nuxt-link>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>
export default {
  name: 'MachineAComponent'
}
</script>
