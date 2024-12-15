<script setup>
import ProfilePic from "@/assets/images/picofme.png";
defineProps({
  //
});
</script>

<template>
    <section class="WhoAmI">
        <div
    class="container flex flex-col items-center justify-center py-16 mx-auto my-8 space-y-5"
  >
    <div class="profile-avatar">
      <img :src="ProfilePic" class="w-52" alt="" />
    </div>

    <div class="font-bold text-center capitalize name-and-designation">
      <h3 class="text-3xl sm:text-4xl">behram khattak</h3>
      <br>
      <span class="text-xl sm:text-2xl"> software engineer - web </span>
    </div>

    <div class="social-links">
      <ul class="flex space-x-10">
        <li>
          <a target="_blank" class="text-blue-500" href="https://twitter.com/behramkttk">
            <font-awesome-icon icon="fab fa-twitter" size="2xl" />
          </a>
        </li>

        <li>
          <a target="_blank" class="text-gray-600" href="https://github.com/Behram-Khattak">
            <font-awesome-icon icon="fab fa-github" size="2xl" />
          </a>
        </li>

        <li>
          <a target="_blank" class="text-blue-500" href="https://www.linkedin.com/in/behramkttk">
            <font-awesome-icon icon="fab fa-linkedin" size="2xl" />
          </a>
        </li>

        <li>
          <a target="_blank" class="text-red-500" href="https://www.youtube.com/@CodeWithBehram7497">
            <font-awesome-icon icon="fab fa-youtube" size="2xl" />
          </a>
        </li>
      </ul>
    </div>
  </div>
    </section>
</template>

<script>
export default {
  //
};
</script>
