<script setup lang="ts">
import { VPTeamMembers } from 'vitepress/theme'
import { teamMembers } from '../contributors'
import Contributors from './Contributors.vue';
</script>

<template>
  <div class="content">
    <div class="content-container">
      <main class="main">
        <div class="vp-doc" flex flex-col items-center mt-10>
          <h2 id="meet-the-team" op50 font-normal p="t-10 b-2">
            Meet The Team
          </h2>
          <div w-full p-10>
            <VPTeamMembers size="medium" :members="teamMembers" />
          </div>
          <h2 id="the-team" op50 font-normal pt-5 pb-2>
            Contributors
          </h2>
          <p text-lg max-w-200 text-center leading-7>
            <Contributors />
            <br>
          </p>
        </div>
      </main>
    </div>
  </div>
</template>
