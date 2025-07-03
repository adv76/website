<script lang="ts">
    import { Canvas, T } from "@threlte/core";
    import { OrbitControls, Stars } from "@threlte/extras";
</script>

<Canvas>
    <Stars />

    <T.PerspectiveCamera
        makeDefault
        position.y={1}
        position.z={8}
        fov={90}>

        <OrbitControls
            enableDamping
            enablePan={false}
            enableZoom={false}
            autoRotateSpeed={0.5}
            autoRotate
        />
    </T.PerspectiveCamera>
</Canvas>

<div class="fixed bottom-0 right-0 z-50 p-2">
    <div class="text-8xl font-bold font-mono tracking-widest bg-[url(/american_flag.png)] bg-clip-text bg-cover bg-center text-transparent">ADV76</div>
</div>
