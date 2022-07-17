<template>
  <div>
    <!-- <vue-qr :correct-level="3" :auto-color="false" color-dark="#313a90" :bg-src="bgSrc" :logo-src="logoSrc" :text="codeUrl" :size="95" :margin="0" :logo-margin="3" /> -->
    <!-- <vue-qr :text="downloadData.url" :margin="0" colorDark="#f67b29" colorLight="#fff" :logoSrc="downloadData.icon + '?cache'" :logoScale="0.3" :size="200"></vue-qr> -->
    <vue-qr text="Hello world!" :callback="test" qid="testid" />
  </div>
</template>
<script>
import VueQr from 'vue-qr'
export default {
  components: {
    VueQr
  },
  data() {
    return {
      // logoSrc: require('../assets/img/qrlogo.png'),
      // bgSrc: require('../assets/img/bgSrc.png'),
      // codeUrl: 'https://github.com/lx719679895'
    }
  },
  methods: {
    test(dataUrl, id) {
      console.log(dataUrl, id)
    }
  }
}
</script>
