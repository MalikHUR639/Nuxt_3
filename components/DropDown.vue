<script setup lang="ts">
const items = [
  [
    {
      label: "USA",
      click: () => {
        updateUrl("en-usa");
      },
    },
  ],
  [
    {
      label: "UK",
      click: () => {
        updateUrl("en-uk");
      },
    },
  ],
  [
    {
      label: "China",
      click: () => {
        updateUrl("en-cn");
      },
    },
  ],
  [
    {
      label: "Pakistan",
      click: () => {
        updateUrl("en-pk");
      },
    },
  ],
];

const updateUrl = (segment:any) => {
  const currentPath = window.location.href;
  var newUrl = currentPath.includes("en")
    ? currentPath.replace(/\/en[^/]*$/, `/${segment}`)
    : currentPath + segment;
  window.location.href = newUrl;
};
</script>

<template>
    
  <UDropdown
    :items="items"
    :popper="{ placement: 'bottom-start' }"
  >
    <UButton color="white" :class="['custom-button','hover:cursor-pointer']" label="Regions" />
  </UDropdown>
</template>

<style scoped>
.custom-button {
  background: radial-gradient(
      163.75% 163.75% at 23.45% 140%,
      #0025ce 0%,
      rgba(9, 93, 230, 0.53) 100%
    ),
    linear-gradient(
      180deg,
      rgba(255, 255, 255, 0.46) 0%,
      rgba(255, 255, 255, 0) 100%
    );
  border-radius: 100px;
  border: 1px solid;
  border-image-source: linear-gradient(
    180deg,
    rgba(255, 255, 255, 0.46) 0%,
    rgba(255, 255, 255, 0) 100%
  );
  box-shadow: 0px 9px 15px 0px #0d93ef inset;
  color: white;
  padding: 10px 50px;
  font-size: 16px;
  font-weight: 500;
  line-height: 19px;

  @media screen and (max-width: 768px) {
    padding: 8px 25px;
    font-size: 14px;
  }

  @media screen and (max-width: 480px) {
    padding: 6px 20px;
    font-size: 12px;
  }
}
</style>
