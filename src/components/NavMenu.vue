<script setup>
import { onMounted, ref,h } from "vue";
import { UnorderedListOutlined,RightOutlined } from "@ant-design/icons-vue"

const mainNav = ref(false)
const sidebar = ref(false)
const items = [
  {
    key: 'home',
    label: 'Home',
    title: 'Home',
    icon: () => h(RightOutlined ),
    path: '/#homesection',
  },
  {
    key: 'about',
    label: 'About',
    title: 'About',
    icon: () => h(RightOutlined),
    path: '/#about_section',
  },
  {
    key: 'skill',
    label: 'Skill',
    title: 'Skill',
    icon: () => h(RightOutlined),
    path: '/#skill_section',
  },
  {
    key: 'project',
    label: 'Project',
    title: 'Project',
    icon: () => h(RightOutlined),
    path: '/#project_section',
  },
  {
    key: 'contact',
    label: 'Contact',
    title: 'Contact',
    icon: () => h(RightOutlined),
    path: '/#contact_section',
  },
];
function checkScreenSize() {
  if (window.innerWidth < 768) {
    mainNav.value = true;
  }
}

onMounted(() => {
  checkScreenSize();
  window.addEventListener("resize", checkScreenSize);
});
const showNav = ()=>{
    sidebar.value = true
}
const closeNav = ()=>{
    sidebar.value = false
}
const toggleMenu = () => {
    sidebar.value = !sidebar.value;
};
</script>
<template>
    <div v-if="!mainNav" class="w-full h-20 flex justify-center items-center shadow-md" id="nav-main-div">
        <nav class="flex space-x-8">
            <li class="font-bold hover:text-orange-600 text-white">
                <a href="#homesection">Home</a>
            </li>
            <li class="font-bold hover:text-orange-600 text-white">
                <a href="#about_section">About</a>
            </li>
            <li class="font-bold hover:text-orange-600 text-white">
                <a href="#skill_section">Skill</a>
            </li>
            <li class="font-bold hover:text-orange-600 text-white">
                <a href="#project_section"> Project</a>
            </li>
            <li class="font-bold hover:text-orange-600 text-white">
                <a href="#contact_section">Contact</a>
            </li>
        </nav>
    </div>
    <div v-else class="w-full bg-white h-10 flex justify-end pr-2 items-center" id="second-div-nav">
        <UnorderedListOutlined class="text-white w-5 text-2xl mr-3" @click="toggleMenu"/>
    </div>
    <a-menu v-if="sidebar" :open="sidebar" :items="items" mode="inline" left :style="{ left: sidebar ? 0 : '-100%' }" />
</template>

<style  scoped>
li{
    list-style-type: none;
}

li .active-link{
    border-bottom: 3px solid rgb(255, 106, 0);
}
#nav-main-div,#second-div-nav{
    background-image: linear-gradient(360deg,rgb(0,0,0,0.8),rgb(0,0,0,0.8)),url('../assets/nav-bg.jpeg');
    background-repeat: no-repeat;
    background-size: cover;
}
</style> 