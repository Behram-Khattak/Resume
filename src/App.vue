<script setup>
import Header from '@/components/Header.vue';
import Footer from '@/components/Footer.vue';
import ComputerGuy from '@/assets/svg/computers_guy_updated.svg';
import ProfilePic2 from '@/assets/images/picofme (2).png';

import { onMounted } from 'vue'
import { initFlowbite } from 'flowbite'

// initialize components based on data attribute selectors
onMounted(() => {
    initFlowbite();
});
</script>

<template>
  <header>
    <div class="wrapper">
      <Header />
    </div>
  </header>

  <main>
    <section class="WhoAmI">
      <div class="container mx-auto flex flex-col items-center py-16" id="whoAmI">
        <div class="title capitalize space-y-5 text-center">
          <h2>hi, i'am</h2>
          <h1>a full stack <span>web engineer</span></h1>
        </div>
        
        <div class="caption mt-5">
          <small>talk's about code...</small>
        </div>
        
        <div class="social-links mt-10">
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

        <div class="computer-guy mt-10">
          <img :src="ComputerGuy" alt="computer-guy-svg">
        </div>
      </div>
    </section>

    <section class="AboutMe">
      <div class="container mx-auto flex flex-col items-center justify-center space-y-5 py-16" id="aboutMe">
        <div class="section-title capitalize text-center">
          <h1>{about me}</h1>
        </div>

        <div class="section-content lg:grid grid-cols-2 items-center space-y-5 md:space-x-5">
          <div class="profile-pic flex justify-center">
              <img :src="ProfilePic2" class="w-96" alt="">
          </div>

          <div class="vs-code rounded-2xl p-5 overflow-hidden">
            <div class="mac-toolbar flex space-x-3 mb-10">
              <div class="sphere"></div>
              <div class="sphere"></div>
              <div class="sphere"></div>
            </div>

            <p class="journey-text md:text-xl lg:text-2xl
                first-letter:text-7xl first-letter:font-bold first-letter:mr-3"
            >
              Hi, this is <a href="/" class="font-bold text-red-500">Behram Khattak</a>, a Full Stack Web Engineer from Pakistan. Who loves to find solution to complicated problems. I do Web development and designing and also a bit of UI/UX designing. My personal favourite programming language is PHP. Why ? Because it's just simple to configure, connect and to play with. I also teach Web development tips and tricks on my youtube channel. 
              <a target="_black" href="https://www.youtube.com/channel/UCtOp_as72Gcnj1xN9CpkLow" class="hover:text-red-500">
                <font-awesome-icon icon="fab fa-youtube" size="xl"/>
              </a>
            </p>
            
            <a href="#approachMe" class="approach-me-btn p-2 rounded-full capitalize text-sm float-right font-bold">
                approach me
                <font-awesome-icon icon="fas fa-phone"/>
            </a>
          </div>
        </div>
      </div>

    </section>

    <section class="MyJourney">
      <div class="container mx-auto flex flex-col items-center justify-center space-y-5 py-16" id="myJourney">
        <div class="section-title capitalize text-center">
          <h1>{my journey}</h1>
        </div>

        <div class="section-content">
          <!-- component -->
          <div class="main-skills">
            <div class="py-3 sm:max-w-xl sm:mx-auto w-full px-2 sm:px-0">
              <div class="relative antialiased text-sm font-semibold capitalize">
                <!-- Vertical bar running through middle -->
                <div class="timeline-vertical-bar rounded hidden sm:block w-1 absolute h-full left-1/2 transform -translate-x-1/2"></div>

                <!-- Left section, set by justify-start and sm:pr-8 -->
                <div class="mt-6 sm:mt-0 sm:mb-12">
                  <div class="flex flex-col sm:flex-row items-center">
                    <div class="flex justify-start w-full mx-auto items-center">
                      <div class="w-full sm:w-1/2 sm:pr-8">
                        <div class="p-4 rounded-xl border border-red-500">
                          <span class="text-xl text-red-500">php</span><br>
                          Started learning Php back in 2019.  and still looking for implementing new ideas that can speed up the development as well as the afterwords website life to the next level. Php is my all-time favorite General Purpose language. Php also acquires almost half of the web and is the most suitable language for web apps.
                        </div>
                      </div>
                    </div>
                    <div class="rounded-full bg-red-500 border-white border-4 w-8 h-8 absolute left-1/2 -translate-y-4 sm:translate-y-0 transform -translate-x-1/2 flex items-center justify-center">
                      <font-awesome-icon icon="fab fa-php"/>
                    </div>
                  </div>
                </div>

                <!-- Right section, set by justify-end and sm:pl-8 -->
                <div class="mt-6 sm:mt-0 sm:mb-12">
                  <div class="flex flex-col sm:flex-row items-center">
                    <div class="flex justify-end w-full mx-auto items-center">
                      <div class="w-full sm:w-1/2 sm:pl-8">
                        <div class="p-4 rounded-xl border border-red-500">
                          <span class="text-xl text-red-500">javascript</span><br>
                          Started learning Javascript back in 2019, and still working with Frameworks like Vue and React. These frameworks make the complicated work so much easy for the developers out there.
                        </div>
                      </div>
                    </div>
                    <div class="rounded-full bg-red-500 border-white border-4 w-8 h-8 absolute left-1/2 -translate-y-4 sm:translate-y-0 transform -translate-x-1/2 flex items-center justify-center">
                      <font-awesome-icon icon="fab fa-js"/>
                    </div>
                  </div>
                </div>

                <!-- Left section, set by justify-start and sm:pr-8 -->
                <div class="mt-6 sm:mt-0 sm:mb-12">
                  <div class="flex flex-col sm:flex-row items-center">
                    <div class="flex justify-start w-full mx-auto items-center">
                      <div class="w-full sm:w-1/2 sm:pr-8">
                        <div class="p-4 rounded-xl border border-red-500">
                          <span class="text-xl text-red-500">frameworks</span><br>
                          Started learning Frameworks like Laravel, React, and Vue back in 2021, and still working with these Frameworks creating projects like:
                          (CMS) Content Management Systems
                          Custom E-commerce Platforms
                          Chat Applications
                          (LMS) Learning Management Systems
                        </div>
                      </div>
                    </div>
                    <div class="rounded-full bg-red-500 border-white border-4 w-8 h-8 absolute left-1/2 -translate-y-4 sm:translate-y-0 transform -translate-x-1/2 flex items-center justify-center">
                      <font-awesome-icon icon="fas fa-box"/>
                    </div>
                  </div>
                </div>

                <!-- Right section, set by justify-end and sm:pl-8 -->
                <div class="mt-6 sm:mt-0">
                  <div class="flex flex-col sm:flex-row items-center">
                    <div class="flex justify-end w-full mx-auto items-center">
                      <div class="w-full sm:w-1/2 sm:pl-8">
                        <div class="p-4 rounded-xl border border-red-500">
                          <span class="text-xl text-red-500">version control | OS</span><br>
                          Started using Linux Ubuntu back in 2021. Linux really speed up my development career. Also Recently Started learning how Docker works and looking forward to use in my development career.
                        </div>
                      </div>
                    </div>
                    <div class="rounded-full bg-red-500 border-white border-4 w-8 h-8 absolute left-1/2 -translate-y-4 sm:translate-y-0 transform -translate-x-1/2 flex items-center justify-center">
                      <font-awesome-icon icon="fas fa-server"/>
                    </div>
                  </div>
                </div>

              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <hr class="border-gray-500 text-center">

    <section class="MyArts">
      <div class="container mx-auto flex flex-col items-center justify-center space-y-5 py-16" id="myArts">
        <div class="section-title capitalize text-center">
          <h1>{my Arts}</h1>
        </div>

        <div class="section-content">
          <div class="grid sm:grid-cols-2 lg:grid-cols-3 gap-10">
            <div class="arts-item p-5 rounded-2xl capitalize">
              <a href="https://quotes.network" target="__blank">
                <h5 class="font-bold text-2xl arts-title pb-2 underline">quotes.network</h5>
              </a>
              <p>
                Join Us On Our Engaging Social Media Journey As We Curate And Share The Best Quotes Every Day. Connect With Us On Pinterest And Instagram To Enhance Your Personal Growth And Enrich Your Daily Life.
              </p>
              <div class="pt-4 pb-2 arts-keywords">
                <small class="inline-block rounded-full px-3 py-1 font-semibold mr-2 mb-2">#laravel</small>
                <small class="inline-block rounded-full px-3 py-1 font-semibold mr-2 mb-2">#bootstrap</small>
                <small class="inline-block rounded-full px-3 py-1 font-semibold mr-2 mb-2">#javascript</small>
              </div>
            </div>

            <div class="arts-item p-5 rounded-2xl capitalize">
              <a href="https://cogni4health.com/" target="__blank">
                <h5 class="font-bold text-2xl arts-title pb-2 underline">cogni 4 health</h5>
              </a>
              <p>
                Cogni® is expanding Wellness for All, Always Providing virtual solutions to accelerate wellness results so that Wellness Programs and Mental Health Providers support more people without delay.
              </p>
              <div class="pt-4 pb-2 arts-keywords">
                <small class="inline-block rounded-full px-3 py-1 font-semibold mr-2 mb-2">#laravel</small>
                <small class="inline-block rounded-full px-3 py-1 font-semibold mr-2 mb-2">#bootstrap</small>
                <small class="inline-block rounded-full px-3 py-1 font-semibold mr-2 mb-2">#javascript</small>
              </div>
            </div>
          </div>
        </div>
      </div>
    </section>

    <section class="ApproachMe">
      <div class="container mx-auto flex flex-col items-center justify-center space-y-10 py-16" id="approachMe">
        <div class="section-title capitalize text-center">
          <h1>{approach me}</h1>
        </div>

        <div class="section-content">
          <div class="approach-me-methods grid lg:grid-cols-2 lg:gap-60 capitalize">
          <div class="call flex items-center space-x-5">
            <span class="approach-me-icons">
              <font-awesome-icon icon="fas fa-mobile" size="5x"/>
            </span>

            <span class="font-bold">
              business call <br>
              <a href="tel:+923319218866" class="underline">
                +923319218866
              </a>
            </span>

          </div>
          
          <div class="mail flex items-center space-x-5 my-10">
            <span class="approach-me-icons">
              <font-awesome-icon icon="fas fa-envelope" size="5x"/>
            </span>

            <span class="font-bold">
              business mail <br>
              <a href="mailto:behramkttk9@gmail.com" target="_blank" class="underline">
                behramkttk9@gmail.com
              </a>
            </span>
          </div>
          </div>
        </div>
      </div>
    </section>

  </main>

  <footer>
    <Footer />
  </footer>
</template>

<script>
  export default {
    // 
  };
</script>
