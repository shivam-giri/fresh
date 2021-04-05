<template>
  <div class="">
    <div >
        <h3 class="p-3 border-b">Add Coupon Code</h3>
        <div class="p-5 flex flex-row">
         <label
            class="flex flex-col p-3  bg-white border-2 w-1/4 mr-6 rounded shadow cursor-pointer hover:shadow-lg"
            :class="{ 'border-blue-500 bg-blue-100': picked == 'one' }"
          >
            <div class="flex flex-row">
              <input
                type="radio"
                name="group"
                class="w-4 h-4 my-auto mr-3 "
                v-model="picked"
                value="one"
              />
              <span class="flex flex-row text-gray-500 ">
                Single Coupon Code
              </span>
            </div>
          </label>
           <label
            class="flex flex-col p-3  bg-white border-2 w-1/4 rounded shadow cursor-pointer hover:shadow-lg"
            :class="{ 'border-blue-500 bg-blue-100': picked == 'Two' }"
          >
            <div class="flex flex-row">
              <input
                type="radio"
                name="group"
                class="w-4 h-4 my-auto mr-3 "
                v-model="picked"
                value="Two"
              />
              <span class="flex flex-row text-gray-500">
                Bulk Coupon Code
              </span>
            </div>
          </label>
        </div>
        <div class="p-5">
          <div class="flex flex-col">
            <span class="mr-3 mb-1 my-auto">Enter Name</span>
            <input
                type="text"
                id="text"
                placeholder="Input Text"
                autofocus
                required
                class="px-4 py-2 transition duration-300 border-none rounded focus:ring-1 focus:ring-yellow-600 ring-1 ring-gray-400 focus:border-transparent focus:outline-none"
              />
          </div>
          <div class="flex flex-col mt-3">
            <span class="mr-3 mb-1 my-auto">Enter Coupon Code</span>
            <input
                type="text"
                id="text"
                placeholder="Input Text"
                autofocus
                required
                class="px-4 py-2 transition duration-300 border-none rounded focus:ring-1 focus:ring-yellow-600 ring-1 ring-gray-400 focus:border-transparent focus:outline-none"
              />
          </div>
        </div>
        <div class="p-5">
          <h3 class="font-medium">Type Of Discount</h3>
          <div class="flex flex-row w-full">
            <div class="w-1/4 mt-2">
              <input class="my-3" type="radio" id="one" value="1" v-model="picked">
                <label for="one">Percentage Discout</label>
              <br>
              <input class="my-3" type="radio" id="two" value="two" v-model="picked">
                <label for="two">Fixed Amount Discout</label>
            </div>
            <div class="w-1/3">
              <input
                type="text"
                id="text"
                placeholder="Enter Discount"
                autofocus
                required
                class="px-4 py-2 border border-gray-400 shadow rounded focus:border-transparent"
              />
            </div>
          </div>

        </div>
    </div>
  </div>
</template>

<script>
export default {
  data(){
    return{
      picked: null
    }
  }
}
</script>
<style>

.NuxtLogo {
  animation: 1s appear;
  margin: auto;
}

@keyframes appear {
  0% {
    opacity: 0;
  }
}
</style>
