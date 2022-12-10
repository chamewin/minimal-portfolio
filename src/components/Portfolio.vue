<script setup lang="ts">
import portfolio from '../data/portfolio';
</script>

<template>
  <div className="flex flex-col md:flex-row items-center justify-center">
    <div className="grid grid-cols-1 md:grid-cols-2 lg:grid-cols-3 gap-4 m-8">
      <div
        v-for="project in portfolio"
        className="border-2 border-stone-900 rounded-md overflow-hidden"
      >
        <img
          src="{{ project.imgUrl }}"
          alt=""
          className="w-full h-36 md:h-48 object-cover cursor-pointer"
        />
        <div className="w-full p-4">
          <h3 className="text-lg md:text-xl mb-2 md:mb-3 font-semibold">
            {{ project.title }}
          </h3>
          <p
            className="flex flex-wrap gap-2 flex-row items-center justify-start text-xs md:text-sm"
          >
            <span
              v-for="item in project.stack"
              className="inline-block px-2 py-1 font-semibold border-2 border-stone-900 rounded-md"
            >
              {{ item }} &nbsp;
            </span>
          </p>
        </div>
      </div>
    </div>
  </div>
</template>
