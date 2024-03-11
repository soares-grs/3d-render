<script setup>

</script>

<template>
    <div class="flex justify-center h-full w-full">
        <div class="absolute h-full top-0 w-full">
            <ClientOnly>
                <LazyPc class="cursor-pointer"/>
            </ClientOnly>
        </div>
        <h1 class="text-2xl m-4 font-bold text-white">My Super Computer</h1>
    </div>
</template>