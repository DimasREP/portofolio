<script setup>
import { Navbar, NavbarLogo, NavbarCollapse, NavbarLink } from "flowbite-vue";
</script>
<template>
  <Navbar>
    <template #logo>
      <NavbarLogo
        link="https://www.google.com/"
        alt=""
        image-url="https://img.freepik.com/free-icon/user_318-180888.jpg?size=626&ext=jpg&ga=GA1.1.353176421.1690346064&semt=ais">
        Dimass.
      </NavbarLogo>
    </template>
    <template #default="{ isShowMenu }">
      <NavbarCollapse :isShowMenu="isShowMenu">
        <NavbarLink is-active>Home</NavbarLink>
        <NavbarLink link="#about">Tentang</NavbarLink>
        <NavbarLink link="#skill">Skill</NavbarLink>
        <NavbarLink link="#project">Project</NavbarLink>
      </NavbarCollapse>
    </template>
    <template #right-side>
      <button
        type="button"
        class="text-white bg-blue-700 hover:bg-blue-800 focus:ring-4 focus:outline-none focus:ring-blue-300 font-medium rounded-lg text-sm px-5 py-2.5 text-center mr-3 md:mr-0 dark:bg-blue-600 dark:hover:bg-blue-700 dark:focus:ring-blue-800"
      >
        Download CV
      </button>
    </template>
  </Navbar>
</template>
