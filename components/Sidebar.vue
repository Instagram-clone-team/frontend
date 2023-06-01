<template>
    <div class="bg-white w-[335px] h-screen">
        <a href="/">`
            <img class="mt-[16px] ml-[23px] mb-8" src="../public/icons/logo.svg" alt="">
        </a>
        <nuxt-link
            class="{ 'rounded-full': id === roundedImage } flex gap-[16px] p-4 ml-[10px] rounded-xl font-bold hover:bg-gray-100 w-[310px]"
            v-for="el in DashboardLinks">
            <img :src="`/icons/${el.icon}`" alt=""> <span>{{ el.title }}</span>
        </nuxt-link>
        <nuxt-link
            class="{ 'rounded-full': id === roundedImage } flex gap-[16px] p-4 ml-[10px] rounded-xl font-bold hover:bg-gray-100 w-[310px]">
            <img class="rounded-full" src="../public/icons/profile.png" alt=""> <span>Profile</span>
        </nuxt-link>
        <nuxt-link
            class="{ 'rounded-full': id === roundedImage } flex gap-[16px] p-4 ml-[10px] rounded-xl font-bold hover:bg-gray-100 w-[310px]">
            <img class="rounded-full" src="../public/icons/more.svg" alt=""> <span>More</span>
        </nuxt-link>

    </div>
</template>

<script setup>
const DashboardLinks = [
    {
        id: 1,
        title: "Home",
        link: "/Home",
        icon: "home.svg"
    },
    {
        id: 2,
        title: "Search",
        link: "/Search",
        icon: "search.svg"
    },
    {
        id: 3,
        title: "Explore",
        link: "/explore",
        icon: "explore.svg"
    },
    {
        id: 4,
        title: "Reels",
        link: "/reels",
        icon: "reels.svg"
    },
    {
        id: 5,
        title: "Messages",
        link: "/user",
        icon: "messages.svg"
    },
    {
        id: 6,
        title: "Notifications",
        link: "/chat",
        icon: "notifications.svg"
    },
    {
        id: 7,
        title: "Create",
        link: "/lastest_activity",
        icon: "create.svg"
    },
    // {
    //     id: 8,
    //     title: "Profile",
    //     link: "/chat",
    //     icon: "profile.png"
    // },
    // {
    //     id: 9,
    //     title: "More",
    //     link: "/lastest_activity",
    //     icon: "more.svg"
    // }
]

</script>

<style lang="scss" scoped></style>