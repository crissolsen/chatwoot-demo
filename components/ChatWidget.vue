<template></template>

<script>
export default {
  mounted() {
    (function(d,t) {
        var BASE_URL="https://hc-chatwoot-demo.herokuapp.com";
        var g=d.createElement(t),s=d.getElementsByTagName(t)[0];
        g.src=BASE_URL+"/packs/js/sdk.js";
        g.defer = true;
        g.async = true;
        s.parentNode.insertBefore(g,s);
        g.onload=function(){
          window.chatwootSDK.run({
            websiteToken: 'daxYxHbuzP3kebMDH27AZuZY',
            baseUrl: BASE_URL
          })
        }
      })(document,"script");
  },
};
</script>