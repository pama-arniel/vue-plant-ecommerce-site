<template>
  <div class="new-tag">
    <div class="new-text valign-text-middle worksans-normal-scarpa-flow-16px">
      New
    </div>
    <img class="line" :src="line" alt="Line" />
  </div>
</template>

<script>
export default {
  name: "NewLabel",
  props: ["line"],
};
</script>

<style>
.new-tag {
  display: flex;
  flex-direction: column;
  gap: 1px;
  height: 20px;
  min-width: 35px;
}

.new-text {
  height: 16px;
  letter-spacing: 0;
  line-height: 16px;
  white-space: nowrap;
  width: 35px;
}

.line {
  height: 3px;
  width: 35px;
}
</style>
