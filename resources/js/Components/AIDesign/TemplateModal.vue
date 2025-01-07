<template>
  <div class="modal-overlay fixed inset-0 bg-black bg-opacity-50 z-60 overflow-y-scroll">
    <div class="modal-content flex flex-col gap-[42px] bg-white px-[30px] pt-[32px] pb-[64px] rounded-lg max-w-5xl mx-auto my-[95px]">
      <div class="template-modal-header w-full flex justify-between items-center">
        <h1 class="text-xl font-sans1 text-[#2F3144]" @click="closeTemplateModal">Template variations</h1>
        <div class="flex justify-between items-center gap-[48px]">
          <div class="flex justify-around items-center gap-[10px] h-[44px] px-[9px] py-[6px] rounded-[6px] border-[1px] border-[#D0D5DD]">
            <img src="/assets/Image/icon/palette.svg" alt="palette" class="w-[24px] shadow-[0px_2px_4px_0px_rgba(0,0,0,0.2)]" />
            <div class="flex">
              <div class="w-[16px] h-[16px] bg-[#E74A49] border-[1px] border-[#FFFFFF]"></div>
              <div class="w-[16px] h-[16px] bg-[#B7263D] border-[1px] border-[#FFFFFF]"></div>
              <div class="w-[16px] h-[16px] bg-[#F2A481] border-[1px] border-[#FFFFFF]"></div>
              <div class="w-[16px] h-[16px] bg-[#44107D] border-[1px] border-[#FFFFFF]"></div>
            </div>
            <div class="pt-[6px]">
              <svg width="16" height="16" viewBox="0 0 11 10" fill="none" xmlns="http://www.w3.org/2000/svg">
                <mask id="mask0_671_4188" style="mask-type:luminance" maskUnits="userSpaceOnUse" x="0" y="0" width="11" height="7">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M10.3002 0.33805L10.5357 0.587467C10.781 0.847341 10.7799 1.26988 10.5389 1.52523L6.04285 6.28855C6.04206 6.28932 6.04127 6.2901 6.04061 6.291L5.80504 6.54042L5.77039 6.57114L5.7155 6.62033C5.50427 6.77576 5.22321 6.77731 5.00828 6.62111C5.00405 6.61839 4.99995 6.6153 4.99585 6.6122C4.96847 6.5909 4.94188 6.56701 4.91675 6.54042L4.68132 6.291L4.67788 6.28713L0.182873 1.52523C-0.0606264 1.26717 -0.0623458 0.850697 0.186047 0.587467L0.42161 0.33805C0.666829 0.0781766 1.06574 0.0793385 1.30659 0.334565L5.36037 4.62952L9.4152 0.334565C9.6587 0.0766274 10.0518 0.07482 10.3002 0.33805Z" fill="white"></path>
                </mask>
                <g mask="url(#mask0_671_4188)">
                <path fill-rule="evenodd" clip-rule="evenodd" d="M-6.59668 -6.45581H17.3164V14.1589H-6.59668V-6.45581Z" fill="#A8AAB7"></path>
                </g>
              </svg>
            </div>
          </div>
          <div @click="closeTemplateModal" class="cursor-pointer text-[#6245E7]">
            <svg width="12" height="13" viewBox="0 0 12 13" fill="none" xmlns="http://www.w3.org/2000/svg">
              <path d="M7.40994 6.49994L11.7099 2.20994C11.8982 2.02164 12.004 1.76624 12.004 1.49994C12.004 1.23364 11.8982 0.978245 11.7099 0.789941C11.5216 0.601638 11.2662 0.49585 10.9999 0.49585C10.7336 0.49585 10.4782 0.601638 10.2899 0.789941L5.99994 5.08994L1.70994 0.789941C1.52164 0.601638 1.26624 0.49585 0.999939 0.49585C0.733637 0.49585 0.478243 0.601638 0.289939 0.789941C0.101635 0.978245 -0.00415277 1.23364 -0.00415277 1.49994C-0.00415278 1.76624 0.101635 2.02164 0.289939 2.20994L4.58994 6.49994L0.289939 10.7899C0.196211 10.8829 0.121816 10.9935 0.0710478 11.1154C0.0202791 11.2372 -0.00585938 11.3679 -0.00585938 11.4999C-0.00585938 11.632 0.0202791 11.7627 0.0710478 11.8845C0.121816 12.0064 0.196211 12.117 0.289939 12.2099C0.382902 12.3037 0.493503 12.3781 0.615362 12.4288C0.737221 12.4796 0.867927 12.5057 0.999939 12.5057C1.13195 12.5057 1.26266 12.4796 1.38452 12.4288C1.50638 12.3781 1.61698 12.3037 1.70994 12.2099L5.99994 7.90994L10.2899 12.2099C10.3829 12.3037 10.4935 12.3781 10.6154 12.4288C10.7372 12.4796 10.8679 12.5057 10.9999 12.5057C11.132 12.5057 11.2627 12.4796 11.3845 12.4288C11.5064 12.3781 11.617 12.3037 11.7099 12.2099C11.8037 12.117 11.8781 12.0064 11.9288 11.8845C11.9796 11.7627 12.0057 11.632 12.0057 11.4999C12.0057 11.3679 11.9796 11.2372 11.9288 11.1154C11.8781 10.9935 11.8037 10.8829 11.7099 10.7899L7.40994 6.49994Z" fill="#1D2939"></path>
            </svg>
          </div>
        </div>
      </div>

      <div class="w-full px-[8px] py-[10px] bg-[#F2F4F7]">
        <div class="flex justify-between items-center px-[15px] py-[10px] rounded-[6px] bg-white">
          <div class="flex gap-[20px]">
            <img src="/assets/Image/img/tab2/showing-template.png" alt="template" class="w-[92px] shadow-[0px_2px_4px_0px_rgba(0,0,0,0.2)] object-center" />
            <div class="m-auto font-sans1">
              <h4 class="text-[16px] font-[400]">Showing results for your template</h4>
              <p class="text-[14px] font-[400] text-[#344054]">8 template variations created</p>
            </div>
          </div>
          <button class="w-[120px] h-[42px] rounded-[8px] border-[1px] border-primary-color text-primary-color text-[15px] font-[600]">Recreate</button>
        </div>
      </div>

      <div class="flex flex-col gap-[20px]">
        <h4 class="text-[15px] text-[#344054] font-[600]">Select your favourite</h4>
        <div class="templates grid grid-cols-1 sm:grid-cols-1 md:grid-cols-2 lg:grid-cols-3 xl:grid-cols-4 gap-[12px]">
          <div
            v-for="(result, index) in templateImages"
            :key="result.id || index"
            class="relative flex justify-center items-center w-full h-auto bg-[#F2F4F7] px-[17px] py-[28px] rounded-[5px] overflow-hidden group"
          >
            <img :src="result.url" alt="Generated Image" class="object-contain transition-transform duration-300 group-hover:scale-110" />
            <div class="overlay absolute inset-0 bg-black bg-opacity-50 flex justify-end items-start p-3 opacity-0 transition-opacity duration-200 group-hover:opacity-100">
              <div class="w-full h-full mx-auto">
                <!-- Centered Buttons -->
                <div class="absolute inset-0 flex justify-center items-center font-sans1 space-y-4">
                  <div class="flex flex-col items-center space-y-4">
                    <button class="w-[112px] h-[30px] bg-transparent border-[1px] border-white rounded-[5px] p-[5px] text-white text-[14px] font-medium transition-all duration-300">
                      Download
                    </button>
                    <button class="w-[112px] h-[30px] bg-primary-color border-[1px] border-white rounded-[5px] p-[5px] text-white text-[14px] font-medium hover:bg-opacity-90 transition-all duration-300">
                      Open in Editor
                    </button>
                  </div>
                </div>
              </div>
            </div>
          </div>
        </div>
      </div>
    </div>
  </div>
</template>

<script>

export default {
  props: {
    templateImages: Array,
    openGeneratedModal: Boolean,
  },
  methods: {
    closeTemplateModal() {
      this.$emit('closeTemplateModal');
    },
  },
};

</script>
