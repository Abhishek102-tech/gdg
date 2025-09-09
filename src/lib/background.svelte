<script>
    import skyscrapers from "../assets/skyscrapers.webp";
    import { onMount } from 'svelte';
    let parallaxEl;
    onMount(() => {
        const handleScroll = () => {
            if (parallaxEl) {
                parallaxEl.style.transform = `translateY(${window.scrollY * 0.3}px)`;
            }
        };
        window.addEventListener('scroll', handleScroll);
        return () => window.removeEventListener('scroll', handleScroll);
    });
</script>

<div class="parallax-skyscrapers" bind:this={parallaxEl}>
    <img src={skyscrapers} alt="skyscrapers" />
</div>

<style>
.parallax-skyscrapers {
    position: fixed;
    left: 0;
    top: 0;
    width: 100vw;
    height: 100vh;
    z-index: -1;
    pointer-events: none;
    overflow: hidden;
    display: flex;
    justify-content: center;
    align-items: flex-end;
}
.parallax-skyscrapers img {
    width: 100vw;
    height: auto;
    object-fit: cover;
    opacity: 0.85;
    filter: drop-shadow(0 0 40px #800080);
    user-select: none;
    pointer-events: none;
}
</style>