<script setup lang="ts">
import { onLaunch, onShow, onHide } from "@dcloudio/uni-app";
onLaunch(() => {
  console.log("App Launch");
  uni.hideTabBar({});
  plus.screen.lockOrientation("landscape-primary");
  uni.setKeepScreenOn({
	  keepScreenOn: true
  });
  plus.device.setWakelock(true); 
});
onShow(() => {
  console.log("App Show");
});
onHide(() => {
  console.log("App Hide");
});
</script>
<style></style>
