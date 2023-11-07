<script setup>
import { onMounted, ref } from "vue";
import i from "./datas/images.json";
import Footer from "./components/Footer.vue";
import NavBar from "./components/NavBar.vue";
import { Icon } from "@iconify/vue";
const computer = ref([]);
const dataAnalyst = ref([]);

onMounted(() => {
  computer.value = i.slice(0, 1);
});
onMounted(() => {
  dataAnalyst.value = i.slice(1, 2);
});
</script>

<template>
  <div class="bg-[#fff8f8]">
    <div class="container cont h-full mx-auto flex flex-col">
      <NavBar />
      <div class="flex gap-[600px] w-[1660px]">
        <div>
          <h1 class="capitalize my-4 text-4xl font-bold">
            let's create someting exceptional together
          </h1>
          <p class="capitalize my-4">
            tunning idea in to extraordinary designs- your vision, our
            expertize,exeptional rusalts
          </p>
          <button
            class="w-[150px] h-10 rounded-r-full rounded-l-full capitalize my-4 bg-black text-white"
          >
            connect with us
          </button>
        </div>
        <div v-for="image in computer" :key="image.id">
          <img :src="image.img" alt="bo image" />
        </div>
      </div>
      <div class="mt-20">
        <div>
          <div class="mb-5">
            <h1 class="capitalize font-bold text-3xl my-3">
              a proven track record
            </h1>
            <hr class="w-[150px] border border-black" />
          </div>
          <div class="grid grid-cols-5 gap-6 my-4">
            <div class="shadow-sm w-[150px] h-32 border">
              <h1 class="font-bold text-3xl py-3 text-center">15</h1>
              <p class="capitalize mx-2 text-center">years of exprience</p>
            </div>
            <div class="shadow-sm w-[150px] h-32 border">
              <h1 class="font-bold text-3xl py-3 text-center">7%</h1>
              <p class="capitalize mx-2 text-center">
                costomers anr infortune 500 list
              </p>
            </div>
            <div class="shadow-sm w-[150px] h-32 border">
              <h1 class="font-bold text-3xl py-3 text-center">100M $</h1>
              <p class="capitalize mx-2 text-center">value created</p>
            </div>
            <div class="shadow-sm w-[150px] h-32 border">
              <h1 class="font-bold text-3xl py-3 text-center">#2</h1>
              <p class="capitalize mx-2 text-center">
                IT industry on design agency
              </p>
            </div>
            <div class="shadow-sm w-[150px] h-32 border">
              <h1 class="font-bold text-3xl py-3 text-center">100+</h1>
              <p class="capitalize mx-2 text-center">project complated</p>
            </div>
          </div>
        </div>
      </div>
      <div>
        <div>
          <h1 class="capitalize font-bold text-2xl">service we offers</h1>
          <hr class="w-[150px] border border-black my03" />
        </div>
        <div class="w-[1536px] grid grid-cols-2 gap-2">
          <div class="flex w-[700px] border my-3 rounded-md">
            <div class="2/5">
              <img
                src="./logo/data.jpg"
                alt=""
                class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
              />
            </div>
            <div class="pl-5 pr-5">
              <h1 class="capitalize font-bold text-xl mt-5"></h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ea
                natus ullam! Modi ipsum provident veritatis sed exercitationem,
                voluptatum distinctio.
              </p>
              <button
                class="capitalize font-bold w-[120px] h-8 my-5 rounded-lg border mt-4"
              >
                get a quote
              </button>
            </div>
          </div>
          <div class="flex w-[700px] border my-3 rounded-md">
            <div class="2/5">
              <img
                src="./logo/uxui.jpg"
                alt=""
                class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
              />
            </div>
            <div class="pl-5 pr-5">
              <h1 class="capitalize font-bold text-xl mt-5"></h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ea
                natus ullam! Modi ipsum provident veritatis sed exercitationem,
                voluptatum distinctio.
              </p>
              <button
                class="capitalize font-bold w-[120px] h-8 my-5 rounded-lg border mt-4"
              >
                get a quote
              </button>
            </div>
          </div>
          <div class="flex w-[700px] border my-3 rounded-md">
            <div class="2/5">
              <img
                src="./logo/consu.png"
                alt=""
                class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
              />
            </div>
            <div class="pl-5 pr-5">
              <h1 class="capitalize font-bold text-xl mt-5"></h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ea
                natus ullam! Modi ipsum provident veritatis sed exercitationem,
                voluptatum distinctio.
              </p>
              <button
                class="capitalize font-bold w-[120px] h-8 my-5 rounded-lg border mt-4"
              >
                get a quote
              </button>
            </div>
          </div>
          <div class="flex w-[700px] border my-3 rounded-md">
            <div class="2/5">
              <img
                src="./logo/full.jpg"
                alt=""
                class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
              />
            </div>
            <div class="pl-5 pr-5">
              <h1 class="capitalize font-bold text-xl mt-5"></h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ea
                natus ullam! Modi ipsum provident veritatis sed exercitationem,
                voluptatum distinctio.
              </p>
              <button
                class="capitalize font-bold w-[120px] h-8 my-5 rounded-lg border mt-4"
              >
                get a quote
              </button>
            </div>
          </div>
          <div class="flex w-[700px] border my-3 rounded-md">
            <div class="2/5">
              <img
                src="./logo/socia.jpg"
                alt=""
                class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
              />
            </div>
            <div class="pl-5 pr-5">
              <h1 class="capitalize font-bold text-xl mt-5"></h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ea
                natus ullam! Modi ipsum provident veritatis sed exercitationem,
                voluptatum distinctio.
              </p>
              <button
                class="capitalize font-bold w-[120px] h-8 my-5 rounded-lg border mt-4"
              >
                get a quote
              </button>
            </div>
          </div>
          <div class="flex w-[700px] border my-3 rounded-md">
            <div class="2/5">
              <img
                src="./logo/seo.png"
                class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
              />
            </div>
            <div class="pl-5 pr-5">
              <h1 class="capitalize font-bold text-xl mt-5"></h1>
              <p>
                Lorem ipsum dolor sit amet consectetur adipisicing elit. Quis ea
                natus ullam! Modi ipsum provident veritatis sed exercitationem,
                voluptatum distinctio.
              </p>
              <button
                class="capitalize font-bold w-[120px] h-8 my-5 rounded-lg border mt-4"
              >
                get a quote
              </button>
            </div>
          </div>
        </div>
      </div>
      <div class="my-5 w-[1536px] flex justify-center">
        <div class="">
          <div class="my-8">
            <h1 class="font-bold text-xl">Our Progress</h1>
            <hr class="w-[100px] border border-black" />
          </div>
          <div
            class="grid grid-cols-3 mx-[100px] gap-[300px] justify-evenly bg-white w-[1400px] h-[200px]"
          >
            <div
              class="w-[180px] h-[130px] border items-center justify-center flex ml-20 my-9"
            >
              <h1 class="capitalize font-bold text-xl">research</h1>
            </div>
            <div
              class="w-[180px] h-[130px] border items-center justify-center flex my-9"
            >
              <h1 class="capitalize text-center font-bold text-xl">design</h1>
            </div>
            <div
              class="w-[180px] h-[130px] border items-center justify-center flex my-9"
            >
              <h1 class="capitalize text-center font-bold text-xl">build</h1>
            </div>
          </div>
        </div>
      </div>
      <div class="container">
        <div>
          <h1 class="capitalize font-bold text-2xl">our work</h1>
          <hr class="border border-black w-[50px]" />
        </div>
        <div class="flex gap-20">
          <div class="flex">
            <div class="flex w-[400px] border my-3 rounded-md">
              <div class="flex flex-col">
                <div class="2/5">
                  <img
                    src="./logo/ux.jpg"
                    class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
                  />
                </div>
                <div class="pl-5 pr-5">
                  <h1 class="capitalize font-bold text-xl mt-5"></h1>
                  <p>UX design | web development.</p>
                  <div class="my-5 mt-4 flex">
                    <h1 class="capitalize font-bold">View Project</h1>
                    <Icon icon="mynaui:arrow-right" class="mt-2 ml-2" />
                  </div>
                </div>
              </div>
            </div>
          </div>

          <div class="flex w-[400px] border my-3 rounded-md">
            <div class="flex flex-col">
              <div class="2/5">
                <img
                  src="./logo/data ala.jpg"
                  class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
                />
              </div>
              <div class="pl-5 pr-5">
                <h1 class="capitalize font-bold text-xl mt-5"></h1>
                <p>UX design | web development.</p>
                <div class="my-5 mt-4 flex">
                  <h1 class="capitalize font-bold">View Project</h1>
                  <Icon icon="mynaui:arrow-right" class="mt-2 ml-2" />
                </div>
              </div>
            </div>
          </div>
          <div>
            <div class="flex flex-col">
              <div class="2/5">
                <img
                  src="./logo/a.jpg"
                  class="w-[400px] h-[200px] border shadow-sm object-cover rounded-l-md"
                />
              </div>
              <div class="pl-5 pr-5">
                <h1 class="capitalize font-bold text-xl mt-5"></h1>
                <p>UX design | web development.</p>
                <div class="my-5 mt-4 flex">
                  <h1 class="capitalize font-bold">View Project</h1>
                  <Icon icon="mynaui:arrow-right" class="mt-2 ml-2" />
                </div>
              </div>
            </div>
          </div>
        </div>
        <div>
          <div class="w-[1536px] flex justify-center">
            <Icon icon="svg-spinners:3-dots-fade" class="text-3xl" />
          </div>
        </div>
      </div>
      <div>
        <div class="w-[1536px] flex justify-center">
          <h1 class="text-center bg-white border-t border-x w-[200px]">
            our trusted partners
          </h1>
        </div>
        <div class="w-[1536px] bg-white border flex justify-center">
          <div class="grid grid-cols-4 gap-28">
            <div class="w-[100px] h-[100px]">
              <Icon icon="simple-icons:cocacola" class="text-9xl" />
            </div>
            <div>
              <Icon icon="arcticons:abc" class="text-9xl" />
            </div>
            <div>
              <Icon icon="raphael:clock" class="text-9xl" />
            </div>
            <div>
              <img src="./logo/yoko.png" alt="" class="w-[200px] h-[150px]" />
            </div>
          </div>
        </div>
      </div>
      <div
        class="bg-[#250b0b] h-[400px] my-9 grid grid-cols-2 gap-5 mx-20 px-20 items-center"
      >
        <div>
          <img
            src="./logo/mamu.png"
            alt=""
            class="w-[200px] h-[200px] border rounded-md"
          />
          <h1 class="text-white font-bold my-5">Mamush Meshesha</h1>
          <p class="text-white">Self-Learner,at Home</p>
        </div>
        <div>
          <div>
            <h1 class="text-white text-2xl font-bold my-5 capitalize">
              talk to our expert
            </h1>
            <p class="text-white capitalize">
              reach out to learn more about our team delivers high quality
              project
            </p>
          </div>
          <div class="my-5">
            <button
              class="text-white w-[140px] border border-white rounded-l-full rounded-r-full capitalize"
            >
              let's talk
            </button>
          </div>
        </div>
      </div>
      <div class="flex">
        <div class="mt-[50px] mx-10 bg-white">
          <h1 class="my-4 capitalize font-bold text-xl w-3/4">
            our 15 years of achievemnet includes:
          </h1>
          <h1>
            <span class="font-bold text-xl">2400+ </span>procject completed
          </h1>
          <h1 class="my-4">
            <span class="font-bold text-xl">900+ </span>satisfied client
          </h1>
          <h1 class="my-4">
            <span class="font-bold text-xl">16+ </span>countries served
          </h1>
        </div>
        <div class="bg-[#8a8888] absolute ml-[600px] flex flex-col rounded-md">
          <div class="px-8 py-8 flex flex-col">
            <h1 class="capitalize my-3 font-bold text-xl">
              consult with us now
            </h1>
            <input
              type="text"
              name="name"
              id=""
              placeholder="Name"
              class="h-10 w-[260px] rounded-sm shadow-md my-3"
            />
            <input
              type="email"
              name="email"
              id=""
              placeholder="Email"
              class="h-10 w-[260px] rounded-sm shadow-md my-3"
            />
            <input
              type="tel"
              name="phone"
              id=""
              placeholder="Phone Number"
              class="h-10 w-[260px] rounded-sm shadow-md my-3"
            />
            <textarea
              name=""
              id=""
              cols="30"
              rows="5"
              placeholder="Tell Us About Your Project"
            ></textarea>
          </div>
        </div>
        <div>
          <div>
            <Icon
              icon="solar:round-arrow-up-bold"
              class="text-3xl flex items-end ml-[800px] mt-[380px]"
            />
          </div>
        </div>
      </div>
    </div>
    <Footer />
  </div>
</template>
