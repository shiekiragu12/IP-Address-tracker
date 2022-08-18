<template>
  <div class="flex flex-col h-screen max-h-screen">
<!--  Search/ Results-->
    <div class="flex justify-center relative bg-hero-pattern bg-cover px-4 pt-8 pb-32">
<!--    Search INput-->
      <div class="w-full max-w-screen-sm">
        <h1 class="text-white text-center text-3xl pb-4">
          IP ADdress Tracker</h1>
        <div class="flex">
          <input class="flex-1 py-3 px-2 rounded-tl-md rounded-bl-md focus:outline-none" type="text"
          placeholder="Search for any Ip address or leave empty to get your ip info">
          <i class="cursor-pointer bg-black text-white px-4 rounded-tr-md rounded-br-md flex items-center bi bi-chevron-right"></i>
        </div>
      </div>
      <!--    IP Info-->
      <IPinfo/>
    </div>
  </div>
</template>

<script>
// @ is an alias to /src
import IPinfo from "@/components/IPinfo";
export default {
  name: 'HomeView',
  components: {
    IPinfo
  }
}
</script>
