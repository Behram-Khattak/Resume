<script setup>
import ProfilePic from '@/assets/images/picofme.png';

defineProps({
  // 
});
</script>

<template>
  <div class="container mx-auto flex flex-col items-center justify-center space-y-5 py-16">
    <div class="profile-avatar">
      <img :src="ProfilePic" class="w-28" alt="">
    </div>

    <div class="name-and-designation capitalize font-bold text-center">
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

  <div class="copy-right capitalize text-center pb-5">
      <span>&COPY; behram 2023</span>
  </div>
</template>



