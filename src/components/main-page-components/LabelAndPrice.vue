<template>
  <div class="label-and-price-1">
    <div class="label-4 valign-text-middle worksans-normal-green-pea-20px">
      {{ label }}
    </div>
    <div class="price-1 valign-text-middle worksans-semi-bold-green-pea-20px">
      {{ price }}
    </div>
  </div>
</template>

<script>
export default {
  name: "LabelAndPrice",
  props: ["label", "price"],
};
</script>

<style>
.label-and-price-1 {
  align-items: flex-start;
  display: flex;
  flex-direction: column;
  gap: 8px;
  width: fit-content;
}

.label-4 {
  letter-spacing: 0;
  line-height: 20px;
  margin-top: -1px;
  white-space: nowrap;
  width: fit-content;
}

.price-1 {
  letter-spacing: 0;
  line-height: 20px;
  white-space: nowrap;
  width: fit-content;
}
</style>
