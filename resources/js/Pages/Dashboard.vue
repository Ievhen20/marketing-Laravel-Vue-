<script setup>

import { ref } from 'vue'
import AuthenticatedLayout from '@/Layouts/AuthenticatedLayout.vue';
import { templateData } from '@/Utils/ImgData';
import { Head } from '@inertiajs/vue3';

const props = defineProps({
  templateData: Array,
});

</script>

<template>

  <Head title="Dashboard" />

  <AuthenticatedLayout>
    <div class="w-full pt-24 px-[24px]">
      <div class="flex gap-2 flex-col lg:flex-row">
        <SideBar />
        <div class="w-full relative flex flex-row">
          <div 
            ref="blogRef"
            class="w-full px-[21px] py-[23px] min-w-[310px] min-h-[85vh] max-h-[85vh] rounded-[15px] bg-[#FFFFFF] overflow-y-auto z-10 custom-scrollbar"
          >
            <div>
              <div class="flex gap-4 justify-between items-center">
                Design your own brand
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </AuthenticatedLayout>
</template>
