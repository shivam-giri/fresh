<template>
    <div class="bg-gray-100 p-6">
        <div class="bg-white" >
         <CommonPart />
        <div class="p-5 flex flex-col">
            <span>Checked names: {{ checkedNames }}</span>
            <span class="my-3 ">
                <input type="checkbox" id="jack" value="Jack" v-model="checkedNames" />
                <label class="cursor-pointer" for="jack">Limit the number of times the code can be redeemed</label>
            </span>
            <span class="my-3 " >
                <input type="checkbox" id="john" value="John" v-model="checkedNames">
                <label class="cursor-pointer" for="John">Add an expiry date</label>
            </span>
            <span class="my-3 ">
                <input type="checkbox" id="mike" value="Mike"  v-model="checkedNames">
                <label class="cursor-pointer" for="mike">Limit to specific courses</label>
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
data(){
 return{
     checkedNames: []
 }
},
    component:{
        CommonPart
    }
}
</script>
