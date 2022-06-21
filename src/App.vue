<!-- npm run serve -->
<template>
  <div id="app">
    <ProgressBar
      v-for="(item, index) in data"
      :key="index"
      :label="item.label"
      :max="200"
      :data="item.elementData"
    />
  </div>
</template>

<script>
import ProgressBar from "../src/components/ProgressBar.vue";

export default {
  name: "App",
  components: {
    ProgressBar,
  },
  data() {
    return {
      data: [
        {
          label: "Risk of Loss",
          elementData: [
            {
              style: "low",
              name: "Low",
              value: 1,
            },
            {
              style: "middle",
              name: "Middle",
              value: 78,
            },
            {
              style: "high",
              name: "High",
              value: 120,
            },
          ],
        },
        {
          label: "Satisfaction",
          elementData: [
            {
              style: "low",
              name: "Low",
              value: 1,
            },
            {
              style: "middle",
              name: "Middle",
              value: 8,
            },
            {
              style: "high",
              name: "High",
              value: 10,
            },
          ],
        },
        {
          label: "Impact of Loss",
          elementData: [
            {
              style: "low",
              name: "Low",
              value: 40,
            },
            {
              style: "middle",
              name: "Middle",
              value: 144,
            },
            {
              style: "high",
              name: "High",
              value: 16,
            },
          ],
        },
        {
          elementData: [
            {
              style: "low",
              name: "Low",
              value: 140,
            },
            {
              style: "#bee5eb",
              name: "Middle",
              value: 40,
            },
            {
              style: "",
              name: "High",
              value: 16,
            },
          ],
        },
      ],
    };
  },
};
</script>
