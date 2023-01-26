<template>
  <div>
    <Suspense>
      <AsyncCityView />
      <template #fallback>
        <CityViewSkeletonVue />
      </template>
    </Suspense>
  </div>
</template>

<script setup>
import AsyncCityView from "../components/AsyncCityView.vue";
import CityViewSkeletonVue from "../components/CityViewSkeleton.vue";
</script>
