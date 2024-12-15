<script setup>
import ProfilePic from '@/assets/images/picofme.png';

defineProps({
  // 
});
</script>

<template>
  <div class="container flex flex-col items-center justify-center py-16 mx-auto space-y-5">
    <div class="profile-avatar">
      <img :src="ProfilePic" class="w-28" alt="">
    </div>

    <div class="font-bold text-center capitalize name-and-designation">
      <h2 class="text-4xl">behram</h2>

      <span>
        full stack web engineer
      </span>
    </div>

    <div class="social-links">
      <ul class="flex space-x-10">
        <li>
          <a target="_blank" href="https://twitter.com/codewithbehram">
            <font-awesome-icon icon="fab fa-twitter" size="xl"/>
          </a>
        </li>

        <li>
          <a target="_blank" href="https://github.com/Behram-Khattak">
            <font-awesome-icon icon="fab fa-github" size="xl"/>
          </a>
        </li>

        <li>
          <a target="_blank" href="https://www.linkedin.com/in/codewithbehram">
            <font-awesome-icon icon="fab fa-linkedin" size="xl"/>
          </a>
        </li>

        <li>
          <a target="_blank" href="https://codedaynight.blog/">
            <font-awesome-icon icon="fas fa-blog" size="xl"/>
          </a>
        </li>
      </ul>
    </div>
  </div>

  <div class="container flex justify-between px-8 pb-5 mx-auto capitalize copy-right lg:px-0">
      <span>&COPY; behram 2023</span>

      <div class="jump-to-top">
        <a href="#whoAmI" class="px-3 py-2 rounded-full">
          <font-awesome-icon icon="fas fa-arrow-up" size="lg" />
        </a>
      </div>
  </div>
</template>



