<template>
    <div>
        <div class="mx-auto py-4">
            <div class="flex flex-wrap font-bold text-gray-100">
                <div class="text-gray-900 text-xl">Youtube Video</div>
                <div class="bg-green-500 text-xl w-full h-1"></div>
                <div class="w-full mt-4">
                    <RouterLink class="ml-2" btnText="Delete Youtube Video" color="red" url="/account/delete-youtube-video"/>
                    <RouterLink btnText="Add Youtube Video" color="green" url="/account/add-youtube-video"/>
                </div>
            </div>
        </div>
        <div class="flex flex-wrap mb-4">
            <div class="my-1 px-1 w-full md:w-1/2 lg:w-1/2">
            <div class="text-xl text-grey-900">Video Title
                <iframe class="w-full h-60" src="https://www.youtube.com/watch?v=A5ab7U9RVLE"></iframe>
            </div>
        </div>
        </div>
    </div>
</template>
<script setup>
import RouterLink from "@/components/global/RouterLinkButton.vue";
</script>