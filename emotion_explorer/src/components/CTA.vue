<template>
  <div
    class="flex flex-wrap justify-center gap-6 md:gap-20 items-center py-16 mt-10 mb-20 text-center px-5 md:px-0 cta"
  >
    <img src="/start.gif" alt="" class="md:max-w-lg" style="max-width: 23rem" />
    <div class="px-10 py-20">
      <h2 class="text-2xl md:text-3xl font-bold mb-6">
        Ready to Empower Your Brain?
      </h2>
      <p class="text-base md:text-lg mb-8">
        Take the next step and join Smart Study to Change Your Life.
      </p>
      <div class="flex justify-center gap-4">
        <RouterLink
          to="/signup"
          class="font-semibold px-4 py-1 bg-blue-600 hover:bg-blue-800 text-white md:px-8 md:py-3 rounded-full text-base md:text-lg"
        >
          Get Started
        </RouterLink>
        <RouterLink
          to="/signup"
          class="bg-transparent border-2 border-blue-600 px-4 py-1 md:px-8 md:py-3 rounded-full text-base md:text-lg font-semibold hover:bg-blue-600 hover:text-white"
        >
          Join Now
        </RouterLink>
      </div>
    </div>
  </div>
</template>

<style scoped>
@keyframes appear {
  0% {
    opacity: 0;
    transform: scale(0.5);
  }
  60% {
    opacity: 1;
    transform: scale(1.1);
  }
  80% {
    transform: scale(0.98);
  }
  100% {
    transform: scale(1);
  }
}

.cta {
  animation: appear 1.5s ease-out both;
  animation-timeline: view();
  animation-range: entry 0% cover 40%;
}
</style>
