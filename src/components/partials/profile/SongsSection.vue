<template>
    <div>
        <div class="mx-auto py-4">
            <div class="flex flex-wrap font-bold text-gray-100">
                <div class="text-gray-900 text-xl">Songs</div>
                <div class="bg-green-500 text-xl w-full h-1"></div>
                <div class="w-full mt-4">
                    <RouterLink class="ml-2" btnText="Delete Song" color="red" url="/account/delete-song"/>
                    <RouterLink btnText="Add Song" color="green" url="/account/add-song"/>
                </div>
            </div>
        </div>
        <div class="pb-4">
            <SongPlayer />
        </div>
    </div>
</template>
<script setup>
import RouterLink from "@/components/global/RouterLinkButton.vue";
import SongPlayer from "@/components/partials/profile/SongPlayer.vue";
</script>