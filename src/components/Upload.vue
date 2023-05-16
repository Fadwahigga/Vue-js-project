<template>
    <h1 class="font-bold">Upload Document</h1>
    <br />
    <!-- card -->
    <div class="flex gap-5">
        <div class="border-collapse rounded-md shadow-md py-6 px-2 w-32 flex flex-col items-center text-center">
            <img src="" class="w-5 pb-2" />
            <h1 class="text-tertiary-info text-sm">Upload from This Device</h1>
        </div>
        <div class="border-collapse rounded-md shadow-md w-32 py-6 px-2 flex flex-col items-center text-center">
            <img src="" class="w-5 pb-2" />
            <h1 class="text-tertiary-info text-sm">Upload from Google Drive</h1>
        </div>
        <div class="border-collapse rounded-md shadow-md w-32 py-6 px-2 flex flex-col items-center text-center">
            <img src="" class="w-5 pb-2" />
            <h1 class="text-tertiary-info text-sm">Upload from DropBox</h1>
        </div>
        <div class="border-collapse rounded-md shadow-md w-32 py-6 px-2 flex flex-col items-center text-center">
            <img src="" class="w-5 pb-2" />
            <h1 class="text-tertiary-info text-sm">Upload from OneDrive</h1>
        </div>
    </div>
    <br />
    <!-- Drag and Drop -->
    
        <FileDrop class="w-72 h-72" @upload="startUpload" />
   
</template>
  
<script setup lang="ts">
import {defineAsyncComponent} from "vue"

const FileDrop = defineAsyncComponent(()=>import(/*webpackChunkName:"filedrop"*/ "./Filedrop.vue"))

function startUpload(files : File[]) : void
{
    files.map(file => console.log("uploading", file))
}

</script>
  