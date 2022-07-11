<link rel="stylesheet" href="/fonts.css">
<link rel="stylesheet" href="/indexstyle.css">
<script>
import { fade, fly, slide } from 'svelte/transition';
import { onMount } from 'svelte';
let ready = false;
onMount(() => (ready = true));
</script>

<div class = "content">

<div class = "section">
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
    </div>
{/if}

</div>

<div class="section">
<img src = "/quote.png" alt = "quote" style = "width: 75vw; display: block; margin-left: auto; margin-right: auto; margin-top:10vh">
<p style="margin-left:10vw;">
    <b>Lorem ipsum</b> dolor sit amet, consectetur adipiscing elit. Donec tincidunt vulputate convallis. 
    Etiam iaculis eros a ipsum aliquet, nec vulputate magna bibendum. Suspendisse finibus ut nisl nec luctus. 
    Maecenas vel mi eget augue iaculis ornare vitae vel nisl. Nulla facilisi. 
    Mauris hendrerit pharetra felis, a condimentum sem vulputate consectetur.
</p>
<p style="float:right; margin-right:10vw;">
    <b>Lorem ipsum</b> dolor sit amet, consectetur adipiscing elit. Donec tincidunt vulputate convallis. 
    Etiam iaculis eros a ipsum aliquet, nec vulputate magna bibendum. Suspendisse finibus ut nisl nec luctus. 
    Maecenas vel mi eget augue iaculis ornare vitae vel nisl. Nulla facilisi. 
    Mauris hendrerit pharetra felis, a condimentum sem vulputate consectetur.
</p>
</div>

</div>  