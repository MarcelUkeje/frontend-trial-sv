<script lang="ts">
    let {href ="/", textContent="Next"} = $props();
    const baseClasses = "w-[70%] bg-black py-2 text-white text-center inline-block cursor-pointer rounded-full";
</script>

<a {href} class={baseClasses}>{textContent}</a>
