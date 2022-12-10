<script setup lang="ts">
import timeline from '../data/timeline';
</script>

<template>
  <div className="flex flex-col md:flex-row justify-center my-20 mx-10">
      <div className="w-full md:w-7/12">
        <!-- Start TimelineItem -->
        <div v-for="point in timeline">
          <ol className="flex flex-col md-flex-row relative border-1 border-stone-200">
            <li className="mb-10 ml-4">
              <div className="absolute w-3 h-3 bg-stone-200 rounded-full mt-1.5 -left-1.5 border border-white" />
              <p className="flex flex-wrap gap-4 flex-row items-center justify-start text-xs md:text-sm">
                <span className="inline-block px-2 py-1 font-semibold text-white bg-stone-900 rounded-md">
                  {{ point.year }}
                </span>
              <h3 className="text-lg font-semibold text-stone-900">
                {{ point.title }}
              </h3>
              <div className="my-1 text-sm font-normal leading-none text-stone-400">
                {{ point.duration }}
              </div>
              </p>
              <p className="my-2 text-base font-normal text-stone-500">
                {{ point.details }}
              </p>
            </li>
          </ol>
        </div>
        <!-- End TimelineItem -->
      </div>
  </div>
</template>

