<template>
  <footer id="contact" class="bg-white">
    <div class="mx-auto w-full max-w-screen-xl p-4 py-6 lg:py-8">
      <hr class="my-6 border-gray-200 sm:mx-auto lg:my-8">
      <div class="md:flex md:justify-between">
        <div class="mb-6 md:mb-0">
          <nuxt-link to="/" class="flex items-center">
            <img src="~/assets/MBL_Logo.png" class="h-8 mr-3" alt="MBL Engineering Logo">
            <span class="self-center text-2xl font-semibold whitespace-nowrap">MBL Engineering</span>
          </nuxt-link>
        </div>
        <div class="grid grid-cols-2 gap-8 sm:gap-6 sm:grid-cols-3">
          <div>
            <h2 class="mb-6 text-sm font-semibold text-gray-900 uppercase">
              Address
            </h2>
            <ul class="text-gray-600 font-medium">
              <li class="mb-4">
                <address>
                  <div>
                    12/2 หมู่ 6 ตำบลห้วยกะปิ
                  </div>
                  <div>อำเภอเมืองชลบุรี จังหวัดชลบุรี 20000</div>
                </address>
              </li>
              <li>
                <address>
                  <a href="https://www.google.co.th/maps/search/1/104+หมู่ที่+2+หนองกะขะ+พานทอง+ชลบุรี+|+บริษัท+เอ.+บี.+ที.+เมทัล+เวิร์ค+จำกัด" target="_blank">
                    <div>
                      1/104 หมู่ที่ 2 ตำบลหนองกะขะ
                    </div>
                    <div>อำเภอพานทอง จังหวัดชลบุรี 20160</div>
                  </a>
                </address>
              </li>
            </ul>
          </div>
          <div>
            <h2 class="mb-6 text-sm font-semibold text-gray-900 uppercase">
              Tel.
            </h2>
            <ul class="text-gray-60 font-medium">
              <li class="mb-4">
                <a href="tel:+66830882681" target="_blank" class="hover:underline">083-088-2681 คุณศุภาวรรณ (มีน)</a>
              </li>
              <li>
                <a href="tel:+66942491529" target="_blank" class="hover:underline">094-249-1529 คุณณภัทร (ตี้)</a>
              </li>
            </ul>
          </div>
          <div>
            <h2 class="mb-6 text-sm font-semibold text-gray-900 uppercase">
              Email & LINE
            </h2>
            <ul class="text-gray-600 font-medium">
              <li class="mb-4">
                <a href="mailto:PUR.MBLENGINEERING@GMAIL.COM" target="_blank" class="hover:underline">PUR.MBLENGINEERING@GMAIL.COM</a>
              </li>
              <li class="mb-4">
                <a href="https://line.me/ti/p/~@309zevgx" target="_blank" class="hover:underline">@309zevgx</a>
              </li>
              <li>
                <img src="~/assets/MBL-LINE.png" class="w-28" alt="line-id">
              </li>
            </ul>
          </div>
        </div>
      </div>
      <div class="mt-6 lg:mt-8 text-sm text-gray-500 text-center">
        จันทร์ - ศุกร์  09:00 - 17:30 น. เสาร์ 09:00 - 13:30 น. ยกเว้นวันหยุดนักขัตฤกษ์
      </div>
      <hr class="my-6 border-gray-200 sm:mx-auto lg:my-8">
      <div class="sm:flex sm:items-center sm:justify-between">
        <span class="text-sm text-gray-500 sm:text-center">บริษัท เอ็มบีแอล เอ็นจิเนียริ่ง จำกัด
        </span>
      </div>
    </div>
  </footer>
</template>

<script>
export default {
  name: 'ContactComponent'
}
</script>
