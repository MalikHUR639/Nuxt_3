<template>
  <section class="py-4 sm:py-6 min-h-screen">
    <div class="container flex flex-col max-w-[1736px] px-5 mx-auto space-y-8">
    
        <Navbar />
        <img
          class="vector z-10"
          src="./public/images/Vector 128.png"
          alt="vector-img"
        />
      
      <div class="text-center">
        <div class="gradient-border-container mt-2 sm:mt-5">
          <p class="text-lg sm:text-xl md:text-2xl font-medium text-white">
            News and Insights
          </p>
        </div>
        <h2 class="text-3xl sm:text-4xl md:text-6xl font-medium mt-4 sm:mt-8">
          <span class="gradient-text">Latest Insights from Leading Voices</span>
        </h2>
        <div class="sm:px-[50px] lg:px-[100px] xl:px-[150px] 2xl:px-[300px]">
        <p
          class="font-serif text-lg sm:text-xl md:text-2xl font-normal text-white mt-2 sm:mt-5"
        >
          Solving the world’s problems through technology wouldn’t be possible
          without our most important invention: the NetSol. Have a look at our
          talented teams.
        </p>
      </div>
        
        <h3 class="text-lg text-white font-normal mt-5">
          <a class="border-b border-white hover:cursor-pointer"
            >View All News</a
          >
        </h3>
      </div>
      <div class="cards-top-margin">
        <div
          class="grid grid-cols-1 gap-x-4 gap-y-8 md:grid-cols-2 xl:grid-cols-4"
        >
          <article class="flex flex-col bg-transparent">
            <a href="#">
              <img
                alt=""
                class="object-cover w-full h-52 bg-transparent aspect-auto"
                src="/images/image 8.png"
              />
            </a>
            <div class="flex flex-col flex-1 py-6 bg-transparent">
              <div
                class="max-w-[70px] gap-[5px] text-center p-[5px] rounded-md bg-[#FFFFFF1A]"
              >
                <p class="text-sm font-bold uppercase text-[#18EBFE]">News</p>
              </div>
              <h3 class="flex-1 py-2 text-2xl font-medium text-white">
                Leasing Life Conference & Awards
              </h3>
              <p class="font-serif text-lg font-normal text-white">
                Solving the world’s problems through technology wouldn’t be
                possible without our most important invention.
              </p>
            </div>
          </article>
          <article class="flex flex-col bg-transparent">
            <a
              href="#"
            >
              <img
                alt=""
                class="object-cover w-full h-52"
                src="./public/images/Rectangle 530.png"
              />
            </a>
            <div class="flex flex-col flex-1 py-6 bg-transparent">
              <div
                class="max-w-[70px] gap-[5px] text-center p-[5px] rounded-md bg-[#FFFFFF1A]"
              >
                <p class="text-sm font-bold uppercase text-[#18EBFE]">News</p>
              </div>
              <h3 class="flex-1 py-2 text-2xl font-medium text-white">
                Auto Finance Summit 2023
              </h3>
              <p class="font-serif text-lg font-normal text-white">
                Solving the world’s problems through technology wouldn’t be
                possible without our most important invention.
              </p>
            </div>
          </article>
          <article class="flex flex-col bg-transparent">
            <a
              href="#"
            >
              <img
                alt=""
                class="object-cover w-full h-52 dark:bg-gray-500"
                src="./public/images/Rectangle 531.png"
              />
            </a>
            <div class="flex flex-col flex-1 py-6 bg-transparent">
              <div
                class="max-w-[70px] gap-[5px] text-center p-[5px] rounded-md bg-[#FFFFFF1A]"
              >
                <p class="text-sm font-bold uppercase text-[#18EBFE]">News</p>
              </div>
              <h3 class="flex-1 py-2 text-2xl font-medium text-white">
                Careers at Netsol
              </h3>
              <p class="font-serif text-lg font-normal text-white">
                Solving the world’s problems through technology wouldn’t be
                possible without our most important invention.
              </p>
            </div>
          </article>
          <article class="flex flex-col bg-transparent">
            <a
              href="#"
            >
              <img
                alt=""
                class="object-cover w-full h-52 dark:bg-gray-500"
                src="./public/images/Rectangle 532.png"
              />
            </a>
            <div class="flex flex-col flex-1 py-6 bg-transparent">
              <div
                class="max-w-[70px] gap-[5px] text-center p-[5px] rounded-md bg-[#FFFFFF1A]"
              >
                <p class="text-sm font-bold uppercase text-[#18EBFE]">News</p>
              </div>
              <h3 class="flex-1 py-2 text-2xl font-medium text-white">
                Leasing Life Conference & Awards
              </h3>
              <p class="font-serif text-lg font-normal text-white">
                Solving the world’s problems through technology wouldn’t be
                possible without our most important invention.
              </p>
            </div>
          </article>
        </div>
      </div>
    </div>
  </section>
</template>

<style>
section {
  background-image: url("./public/images/background.png");
  background-size: cover;
  background-position: center;
}
.gradient-text {
  background: linear-gradient(180deg, #ffffff 49.51%, #c0c0c0 89.32%);
  background-clip: text;
  color: transparent;
}
.gradient-border-container {
  background: linear-gradient(89.97deg, #030a2d -0.5%, #030616 99.97%),
    linear-gradient(90deg, #2b3561 0%, #313651 101.04%);
  border: 1px solid;
  border-image-source: linear-gradient(90deg, #2b3561 0%, #313651 101.04%);
  padding: 10px 20px;
  border-radius: 20px;
  display: inline-block;
  text-align: center;
}
.cards-top-margin {
  margin-top: 60px !important;
}

.tag-bg {
  background: #ffffff1a;
  display: inline-block;
  text-align: start;
}
.vector {
  border-width: 0px, 0px, 0px, 0px;
  border-style: solid;
  border-color: #31364f;
}
@media screen and (max-width: 700px) {
  .cards-top-margin {
    margin-top: 30px !important;
  }
}
</style>
