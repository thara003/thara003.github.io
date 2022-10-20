<template>
  <div class="banner-1">
    <!-- NavBar -->
    <nav class="container px-6 mx-auto md:flex md:justify-between md:items-center">
      <div class="flex items-center justify-between">
        <!-- Mobile menu button -->
        <div @click="showMenu = !showMenu" class="flex md:hidden">
          <button type="button" class="text-gray-800 hover:text-gray-400 focus:outline-none focus:text-gray-400">
            <svg viewBox="0 0 24 24" class="w-6 h-6 fill-current">
              <path fill-rule="evenodd"
                d="M4 5h16a1 1 0 0 1 0 2H4a1 1 0 1 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2zm0 6h16a1 1 0 0 1 0 2H4a1 1 0 0 1 0-2z">
              </path>
            </svg>
          </button>
        </div>
      </div>
      <!-- Mobile Menu open: "block", Menu closed: "hidden" -->
      <ul :class="showMenu ? 'flex' : 'hidden'"
        class="flex-col items-end mt-8 space-y-4 md:flex md:space-y-0 md:flex-row md:items-center md:space-x-10 md:mt-0">
        <li class="menu-button"><a href="#">Home</a></li>
        <li class="menu-button"><a href="#work" v-smooth-scroll>Works</a></li>
        <li class="menu-button"><a href="#about" v-smooth-scroll>About</a></li>
        <li class="menu-button"><a href="#contact" v-smooth-scroll>Contact</a></li>
      </ul>
    </nav>
    <!-- End Navbar -->

    <div class="flex items-center">
      <div class="w-11/12 space-y-5 md:space-y-10">
        <h3
          class="hello-button text-gray-700 w-fit md:py-3 md:px-5 py-1 px-2 rounded-lg 3xl:text-3xl 2xl:text-xl lg:text-xl md:text-md text-sm font-semibold font-work_sans">
          👋 Hola,
        </h3>
        <h1
          class="3xl:text-8xl 2xl:text-7xl xl:text-6xl lg:text-4xl md:text-3xl sm:text-3xl text-xl font-Eczar font-bold leading-tight text-gray-700">
          It's
          <a href="https://github.com/thara003" target="_blank" class="text-black hover:underline">
            Nayan Thara M</a>🙇‍♀️<br />Front-End Developer
        </h1>

        <div class="md:flex gap-1 md:gap-10">
          <a href="#work">
            <button class="text-white bg-gray-800 submit-button hidden md:block">
              View My Work
            </button>
          </a>
          <a href="#contact">
            <button class="text-gray-800 border-4 border-gray-800 submit-button mb-5 md:mb-0">
              Contact Me
            </button>
          </a>
        </div>
      </div>

      <div class="w-8/12 flex justify-end">
        <img class="3xl:h-[800px] 2xl:h-[650px] xl:h-[550px] lg:h-[550px] md:h-[450px] sm:h-[350px]"
          src="./assets/profile-female.png" alt="user image" />
      </div>
    </div>
  </div>

  <div class="banner-2 space-y-10 pb-20" id="work">
    <h3 class="heading3 my-5">My Recent Work</h3>
    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">OONI Probe</h4>
        <p class="font-work_sans pr-12">
          OONI Probe is a free and open-source software designed to measure internet censorship and other forms of network interference.
          I primarily working on the UI/UX of both ther run and the explorer using ReactJS
        </p>
        <a href="https://github.com/ooni">
        <button class="text-sky-800 font-bold text-2xl tracking-wider">
          View Code
        </button>
        </a>
      </div>
      <div class="card-image bg-green-100">
        <img class="object-cover w-full h-72 md:h-96" src="./assets/project1.png" />
      </div>
    </div>

    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title item">Aquilla</h4>
        <p class="font-work_sans pr-12">
          Contributed an open-source academic full stack web app, primarily working on the UI/UX using NextJS, GraphQL,
          and Docker for National Higher Secondary School, Kerala; The project is being currently maintained by my
          organization (THC).
        </p>
        <a href="https://github.com/yeganathan18/aquila">
        <button class="text-sky-800 font-bold text-2xl tracking-wider">
          View Code
        </button>
        </a>
      </div>
      <div class="card-image">
        <img class="object-cover w-full h-48 md:h-96" src="./assets/project2.png" />
      </div>
    </div>

    <div class="card">
      <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
        <h4 class="project-title">Vaquita</h4>
        <p class="font-work_sans pr-12">
          Designed and implemented an Event Management System using Java, SpringBoot, PostgreSQL, HTML/CSS, Bootstrap as
          part of the academic project to be submitted for the university.
        </p>
        <a href="https://github.com/thara003/vaquita">
        <button class="text-sky-800 font-bold text-2xl tracking-wider">
          View Code
        </button>
        </a>
      </div>
      <div class="card-image bg-green-100">
        <img class="object-cover w-full h-72 md:h-96" src="./assets/project1.png" />
      </div>
    </div>
  </div>

  <div class="banner-2 md:flex items-center md:justify-evenly" id="about">
    <img class="md:h-[500px] h-[400px]" src="./assets/about-female.png" alt="user image" />
    <div class="space-y-5 py-8 px-8 md:py-16 md:px-20 md:w-1/2">
      <h4 class="project-title item">Know me</h4>
      <p class="font-work_sans">
        I am a prefinal year student and front-end developer who blends the arts of design and development.
        <br />
        I love applying responsive design principles and watching my web pages shrink into mobile screens and still look
        amazing. It's oddly satisfying. I think in a way I'm kind of like those web pages; I'm moldable, but I still
        keep my creative flair intact.
      </p>
      <button class="text-sky-800 font-bold text-2xl tracking-wider">
        Student by day and hacker by night
      </button>
    </div>
  </div>

  <div class="banner-1 flex h-full items-center" id="contact">
    <div class="w-7/12 p-12">
      <h2 class="text-gray-700 md:text-6xl text-2xl font-Eczar mb-5 font-bold">
        Let’s work together and make everything super cute and super useful.
      </h2>
    </div>
    <div class="w-5/12 pr-28">
      <div class="flex flex-wrap justify-end gap-2">
        <a href="https://github.com/thara003">
          <button class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded">
            <svg xmlns="http://www.w3.org/2000/svg"
              class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current" viewBox="0 0 16 16">
              <path
                d="M8 0C3.58 0 0 3.58 0 8c0 3.54 2.29 6.53 5.47 7.59.4.07.55-.17.55-.38 0-.19-.01-.82-.01-1.49-2.01.37-2.53-.49-2.69-.94-.09-.23-.48-.94-.82-1.13-.28-.15-.68-.52-.01-.53.63-.01 1.08.58 1.23.82.72 1.21 1.87.87 2.33.66.07-.52.28-.87.51-1.07-1.78-.2-3.64-.89-3.64-3.95 0-.87.31-1.59.82-2.15-.08-.2-.36-1.02.08-2.12 0 0 .67-.21 2.2.82.64-.18 1.32-.27 2-.27.68 0 1.36.09 2 .27 1.53-1.04 2.2-.82 2.2-.82.44 1.1.16 1.92.08 2.12.51.56.82 1.27.82 2.15 0 3.07-1.87 3.75-3.65 3.95.29.25.54.73.54 1.48 0 1.07-.01 1.93-.01 2.2 0 .21.15.46.55.38A8.012 8.012 0 0 0 16 8c0-4.42-3.58-8-8-8z" />
            </svg>
          </button>
        </a>
        <a href="https://twitter.com/thara0908">
          <button class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded">
            <svg class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current" role="img"
              xmlns="http://www.w3.org/2000/svg" viewBox="0 0 24 24">
              <path
                d="M23.953 4.57a10 10 0 01-2.825.775 4.958 4.958 0 002.163-2.723c-.951.555-2.005.959-3.127 1.184a4.92 4.92 0 00-8.384 4.482C7.69 8.095 4.067 6.13 1.64 3.162a4.822 4.822 0 00-.666 2.475c0 1.71.87 3.213 2.188 4.096a4.904 4.904 0 01-2.228-.616v.06a4.923 4.923 0 003.946 4.827 4.996 4.996 0 01-2.212.085 4.936 4.936 0 004.604 3.417 9.867 9.867 0 01-6.102 2.105c-.39 0-.779-.023-1.17-.067a13.995 13.995 0 007.557 2.209c9.053 0 13.998-7.496 13.998-13.985 0-.21 0-.42-.015-.63A9.935 9.935 0 0024 4.59z" />
            </svg>
          </button>
        </a>

        <a href="http://linkedin.com/in/nayan-thara-m-9b8586219">
          <button class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded">
            <svg xmlns="http://www.w3.org/2000/svg"
              class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current" viewBox="0 0 16 16">
              <path
                d="M0 1.146C0 .513.526 0 1.175 0h13.65C15.474 0 16 .513 16 1.146v13.708c0 .633-.526 1.146-1.175 1.146H1.175C.526 16 0 15.487 0 14.854V1.146zm4.943 12.248V6.169H2.542v7.225h2.401zm-1.2-8.212c.837 0 1.358-.554 1.358-1.248-.015-.709-.52-1.248-1.342-1.248-.822 0-1.359.54-1.359 1.248 0 .694.521 1.248 1.327 1.248h.016zm4.908 8.212V9.359c0-.216.016-.432.08-.586.173-.431.568-.878 1.232-.878.869 0 1.216.662 1.216 1.634v3.865h2.401V9.25c0-2.22-1.184-3.252-2.764-3.252-1.274 0-1.845.7-2.165 1.193v.025h-.016a5.54 5.54 0 0 1 .016-.025V6.169h-2.4c.03.678 0 7.225 0 7.225h2.4z" />
            </svg>
          </button>
        </a>

        <a href="mailto:nayantharamurukadas@gmail.com">
          <button class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded">
            <svg xmlns="http://www.w3.org/2000/svg"
              class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current" viewBox="0 0 16 16">
              <path
                d="M.05 3.555A2 2 0 0 1 2 2h12a2 2 0 0 1 1.95 1.555L8 8.414.05 3.555ZM0 4.697v7.104l5.803-3.558L0 4.697ZM6.761 8.83l-6.57 4.027A2 2 0 0 0 2 14h12a2 2 0 0 0 1.808-1.144l-6.57-4.027L8 9.586l-1.239-.757Zm3.436-.586L16 11.801V4.697l-5.803 3.546Z" />
            </svg>
          </button>
        </a>

        <a href="tel:7736901669">
          <button class="bg-gray-700 p-2 font-semibold text-white inline-flex items-center space-x-2 rounded">
            <svg xmlns="http://www.w3.org/2000/svg"
              class="w-4 h-4 md:w-10 md:h-10 lg:w-10 lg:h-10 xl:h-10 xl:w-10 fill-current" viewBox="0 0 16 16">
              <path fill-rule="evenodd"
                d="M1.885.511a1.745 1.745 0 0 1 2.61.163L6.29 2.98c.329.423.445.974.315 1.494l-.547 2.19a.678.678 0 0 0 .178.643l2.457 2.457a.678.678 0 0 0 .644.178l2.189-.547a1.745 1.745 0 0 1 1.494.315l2.306 1.794c.829.645.905 1.87.163 2.611l-1.034 1.034c-.74.74-1.846 1.065-2.877.702a18.634 18.634 0 0 1-7.01-4.42 18.634 18.634 0 0 1-4.42-7.009c-.362-1.03-.037-2.137.703-2.877L1.885.511z" />
            </svg>
          </button>
        </a>
      </div>
    </div>
  </div>
</template>
<script>
export default {
  data() {
    return {
      showMenu: false,
    }
  },
}
</script>
