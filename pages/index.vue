<template>
  <div>
    <head>
      <script
        src="https://cdn.onesignal.com/sdks/OneSignalSDK.js"
        async=""
      ></script>
      <script>
        window.OneSignal = window.OneSignal || [];
        OneSignal.push(function() {
          OneSignal.init({
            appId: "d5149721-0cf8-4dd2-8066-f0b1949dd7dc"
          });
        });
      </script>
    </head>
    <Tutorial />
  </div>
</template>

<script>
export default {};
</script>
