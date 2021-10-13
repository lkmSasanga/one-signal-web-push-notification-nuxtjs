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
            appId: "96aff1fa-2988-4e6e-945b-38ac82b1b89c"
          });
        });
      </script>
    </head>
    <h1>One signal web push notification testing project</h1>
  </div>
</template>

<script>
export default {};
</script>
