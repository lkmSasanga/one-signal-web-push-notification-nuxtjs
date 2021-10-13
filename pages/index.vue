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

        // Inside page components
        this.$OneSignal.push(() => {
          this.$OneSignal.isPushNotificationsEnabled(isEnabled => {
            if (isEnabled) {
              console.log("Push notifications are enabled!");
            } else {
              console.log("Push notifications are not enabled yet.");
            }
          });
        });

        // Using window and array form
        window.$OneSignal.push([
          "addListenerForNotificationOpened",
          data => {
            console.log("Received NotificationOpened:", data);
          }
        ]);
      </script>
    </head>
    <h1>One signal web push notification testing project</h1>
  </div>
</template>

<script>
export default {};
</script>
