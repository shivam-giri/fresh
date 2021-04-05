<template>
   <div class="bg-gray-100 p-6">
        <div class="bg-white" >
         <CommonPart />
        <div class="p-5 flex flex-col">
            <span class="my-3 flex flex-col ">
                <div class="flex flex-row">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2 text-green-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                    </svg>
                    <label class="cursor-pointer" for="jack">Limit the number of times the code can be redeemed</label>
                </div>
                <input type="text" class="border border-gray-400 w-1/3 p-1 ml-8 rounded mt-2" id="jack" value="Jack" v-model="checkedNames" />
            </span>
            <span class="my-3 flex flex-col " >
                 <div class="flex flex-row">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2 text-green-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                    </svg>
                    <label class="cursor-pointer" for="John">Limit the number of times the code can be redeemed</label>
                </div>
                <input class="border border-gray-400 p-1 w-1/3 ml-8 rounded mt-2" type="text" id="jack" value="Jack" v-model="checkedNames" />
            </span>
            <span class="my-3 flex flex-col ">
                 <div class="flex flex-row">
                    <svg xmlns="http://www.w3.org/2000/svg" class="h-6 w-6 mr-2 text-green-500" fill="none" viewBox="0 0 24 24" stroke="currentColor">
                        <path stroke-linecap="round" stroke-linejoin="round" stroke-width="2" d="M5 13l4 4L19 7" />
                    </svg>
                    <label class="cursor-pointer" for="mike">Limit the number of times the code can be redeemed</label>
                </div>
                <input class="border border-gray-400 p-1 w-1/3 ml-8 rounded mt-2" type="text" id="jack" value="Jack" v-model="checkedNames" />
            </span>
        </div>
        <div class="w-full flex justify-end p-3">
            <button class="border border-gray-400 px-4 rounded p-2 focus:outline-none mr-3">Cancel</button>
            <button class="border border-blue-500 px-4 rounded bg-blue-500 text-white p-2 focus:outline-none">Save</button>
        </div>
        </div>
    </div>
</template>
<script>
import  CommonPart from '../components/CommonPart'

export default {
    component:{
        CommonPart
    }
}
</script>
