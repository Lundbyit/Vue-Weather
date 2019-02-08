<template>
  <div id="pagecontent"> <!--Position relative -->
    <temp-var-chart :tempVar="tempVar" />
    <today-highlights :highlights="highlights" />
  </div>
</template>

<script>
import TempVarChart from './TempVarChart.vue';
import Highlights from './Highlights.vue';

export default {
  props: ["highlights", "tempVar"],
  components: {
      'temp-var-chart': TempVarChart,
      'today-highlights': Highlights
  }
};
</script>

<style>
</style>

