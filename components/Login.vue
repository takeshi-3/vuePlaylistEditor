<script lang="ts">
import { defineComponent } from 'vue';

export default defineComponent({
    setup() {
        const redirectToLoginURL = (): void => {
            window.location.href = "https://accounts.spotify.com/authorize";
        };

        return {redirectToLoginURL};
    },
})
</script>

<template>
    <div class="flex justify-around py-12">
        <button 
            @click="redirectToLoginURL"
            class="rounded-full shadow-default px-8 py-4 text-green-600 font-bold"
        >
            Sign in with Spotify
        </button>
    </div>
</template>