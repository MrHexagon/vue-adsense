<template>
    <ins class="adsbygoogle"
         :data-ad-client="adClient"
         :data-ad-slot="adSlot"
         :data-full-width-responsive="adFullWidthResponsive"
         :style="adStyle">
    </ins>
</template>

<script>
  export default {
    props: {
      adClient: {
        type: String,
        required: true
      },
      adSlot: {
        type: String,
        required: true
      },
      adFullWidthResponsive: {
        type: String,
        required: false,
        default: 'false'
      },
      adStyle: {
        type: String,
        required: false,
        default: 'display: block'
      }
    },
    mounted() {
      (window.adsbygoogle = window.adsbygoogle || []).push({})
    }
  }
</script>

