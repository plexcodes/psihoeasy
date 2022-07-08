<link rel="stylesheet" href="/fonts.css">
<link rel="stylesheet" href="/indexstyle.css">
<script>
import { fade, fly, slide } from 'svelte/transition';
import { onMount } from 'svelte';
let ready = false;
onMount(() => (ready = true));
</script>

<div class = "content">
<div class = "splashscreen">
        <ul class="circles">
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
                <li></li>
        </ul>
{#if ready}
    <div class="img-front">
        <img  src = "/psihoeasy-splashscreen-logo.png" alt = "logo" style="width:50vw" in:fly={{ y: 500, duration: 2000 }}>
    </div>{/if}
</div>
</div>