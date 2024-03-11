<script setup>

</script>

<template>
    <TresCanvas alpha>
        <TresPerspectiveCamera :position="[-2, 4, 14]"/>
        <OrbitControls :enableZoom="false" :enableDamping="true" :autoRotate="true" :autoRotateSpeed="6" :maxPolarAngle="Math.PI / 2" :minPolarAngle="Math.PI / 2" />
        <TresAmbientLight :intensity="7" />
        <Suspense>
            <GLTFModel path="/pc/scene.gltf" :scale="5" :position="[0, 0, 0]" darco="true" />
        </Suspense>
        <TresDirectionalLight :position="[4, 0, 10]" :intensity="5" cast-shadow />
    </TresCanvas>
</template>