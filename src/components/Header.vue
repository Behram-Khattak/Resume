<script setup>
    defineProps({
        // 
    });
</script>

<template>
    <div class="container mx-auto navigation-bar">
        <nav class="navbar flex justify-between items-center py-5 capitalize">
            <div class="logo">
                <a href="">
                    <h1 class="font-extrabold text-5xl">behram</h1>
                </a>
            </div>

            <div class="nav-links">
                <div class="hamburger cursor-pointer" @click="HamburgerMenu">
                    <div class="bar" :class="{ animate_bar_first:animate_bar_first }"></div>
                    <div class="bar"></div>
                    <div class="bar"  :class="{ animate_bar_last:animate_bar_last }"></div>
                </div>

                <ul class="lg:flex space-x-10 hidden desktop_menus">
                    <li @click="active = 'WhoAmI'">
                        <a href="#whoAmI">
                            <strong  :class="{active:active === 'WhoAmI'}">who am i</strong>
                        </a>
                    </li>
                    <li @click="active = 'aboutMe'">
                        <a href="#aboutMe">
                            <strong :class="{active:active === 'aboutMe'}">about me</strong>
                        </a>
                    </li>
                    <li @click="active = 'myJourney'">
                        <a href="#myJourney">
                            <strong :class="{active:active === 'myJourney'}">my journey</strong>
                        </a>
                    </li>
                    <li @click="active = 'myArts'">
                        <a href="#myArts">
                            <strong :class="{active:active === 'myArts'}">my arts</strong>
                        </a>
                    </li>
                    <li @click="active = 'approachMe'">
                        <a href="#approachMe">
                            <strong :class="{active:active === 'approachMe'}">approach me</strong>
                        </a>
                    </li>
                </ul>
            </div>
        </nav>

    </div>
    
    <!-- Hamburger Mobile Menu -->
    <div :class="{ hidden:hidden }">
        <ul class="hamburger-menu capitalize text-5xl space-y-20 text-center lg:hidden">
            <li @click="HamburgerMenu">
                <a href="#whoAmI">
                    <strong>who am i</strong>
                </a>
            </li>
            <li @click="HamburgerMenu">
                <a href="#aboutMe">
                    <strong>about me</strong>
                </a>
            </li>
            <li @click="HamburgerMenu">
                <a href="#myJourney">
                    <strong>my journey</strong>
                </a>
            </li>
            <li @click="HamburgerMenu">
                <a href="#myArts">
                    <strong>my arts</strong>
                </a>
            </li>
            <li @click="HamburgerMenu">
                <a href="#approachMe">
                    <strong>approach me</strong>
                </a>
            </li>
        </ul>
    </div>

</template>

<script>
    export default {

        data() {
          return { active: null }
        },

        data: () => ({
            hidden: true,
            animate_bar_first: false,
            animate_bar_last: false,
        }),

        methods: {
            HamburgerMenu() {
                this.hidden = !this.hidden;
                this.animate_bar_first = !this.animate_bar_first;
                this.animate_bar_last = !this.animate_bar_last;
            }
        },
    }
</script>