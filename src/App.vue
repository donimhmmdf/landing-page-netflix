<template>
  <header class="container pt-6 w-full lg:flex lg:justify-between">
    <div class="">
      <a href="#" class="">
        <img src="@/assets/logo.png" alt="" class="mx-auto pb-4" />
      </a>
    </div>
    <nav class="lg:flex">
      <ul
        class="flex flex-wrap justify-center lg:justify-start pb-4 items-center"
      >
        <li class="mr-3" v-for="(list, id) in nav" :key="id">
          <a
            href=""
            class="tracking-wide font-semibold text-md lg:text-lg text-white hover:text-primary transition duration-300 ease-in-out"
            >{{ list }}</a
          >
        </li>
      </ul>
    </nav>
    <div class="relative flex items-center">
      <input
        class="lg:w-80 lg:h-10 lg:flex lg:items-center w-full h-full border-2 border-white bg-white bg-opacity-20 backdrop-blur-sm rounded-md py-3 pl-10 border-none outline-none placeholder:text-white placeholder:z-20"
        type="text"
        placeholder="Search..."
      />
      <i
        class="lg:top-7 lg:left-2 fa-sharp fa-solid fa-magnifying-glass text-white absolute left-2 top-4 pr-2 border-r"
      ></i>
    </div>
  </header>

  <div class="banner w-full container pt-8">
    <img src="@/assets/name.png" class="w-60" alt="" />
    <div class="detail text-white flex justify-start">
      <span
        v-for="(detail, id) in details"
        :key="id"
        class="border-r px-3 first:pl-0 last:border-none font-semibold opacity-60"
        >{{ detail }}</span
      >
    </div>
    <div
      class="sinopsis text-white font-medium pt-3 pb-36 lg:w-1/2 text-justify"
    >
      <p class="tracking-wide lg:text-xl text-slate-300">
        Lorem, ipsum dolor sit amet consectetur adipisicing elit. Sunt ab,
        repudiandae ipsam debitis quaerat earum sequi voluptatum vel animi non
        fuga deleniti facere accusantium, ea vitae corrupti atque? Numquam,
        repudiandae?
      </p>
      <button class="flex pt-4 pb-6">
        <a
          href=""
          class="py-2 items-center conte px-5 bg-primary mr-3 rounded-md uppercase font-semibold hover:bg-white hover:text-primary transition duration-300 ease-in-out"
          ><i class="fa-solid fa-play mr-2"></i>Play</a
        >
        <a
          href=""
          class="py-2 px-5 rounded-md bg-slate-700 uppercase font-semibold bg-opacity-60 hover:bg-white transition duration-300 ease-in-out hover:text-slate-700"
          ><i class="fa-solid fa-plus mr-2"></i>My List</a
        >
      </button>
      <a href="" class="flex items-center uppercase font-semibold">
        <img src="@/assets/play.png" class="w-12 mr-3" alt="" /> Watch Trailer
      </a>
    </div>
  </div>
  <div></div>
</template>

<script>
export default {
  name: "App",
  data() {
    return {
      nav: ["Home", "TV Shows", "Movies", "Latest", "My List"],
      details: ["2022", "12+", "1h 55 min", "Action"],
    };
  },
};
</script>
<style></style>
