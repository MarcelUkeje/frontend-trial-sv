<script lang="ts">
	import Header from "$lib/components/Header.svelte";  
	import Footer from "$lib/components/Footer.svelte";

  // import addBlack from "$lib/images/add-black.svg";
  // import arrowLeft from "$lib/images/arrow-left.svg";
  import store from "$lib/images/store.svg";
  import location from "$lib/images/location.svg";
  import phone from "$lib/images/phone.svg";
  // import deleteIcon from "$lib/images/delete.svg";
  import search from "$lib/images/search.svg"
</script>

<svelte:head>
  <title>Screen 41</title>
</svelte:head>

<Header />
<div class="main bg-gray-100 px-4">
  <div class="mt-4 rounded-lg bg-white p-4 shadow-md">
    <p class="font-semibold">Preview</p>
    <div
      class="mt-4 flex flex-col rounded-lg border border-gray-300 p-4"
    >
      <div
        class="flex h-14 w-14 shrink-0 items-center justify-center rounded-full bg-gray-200 p-1"
      >
        <img
          src={store}
          alt=""
          class="h-auto w-6 object-contain"
        />
      </div>
      <p class="font-semibold">Coastal Coffee Co.</p>
      <p class="text-gray-400">Coffee Shop & Bakery</p>
      <div class="flex items-center gap-2">
        <img
          src={location}
          class="h-auto w-4"
          alt=""
        />
        <p class="text-gray-400">123 Ocean Drive, Miami Beach, FL</p>
      </div>
      <div class="flex items-center gap-2">
        <img
          src={phone}
          class="h-auto w-4"
          alt=""
        />
        <p class="text-gray-400">(305) 555-0123</p>
      </div>
    </div>
  </div>
  <div
    class="mt-8 flex flex-col rounded-lg bg-white p-4 shadow-md"
  >
    <label for="business_name" class="font-semibold"
      >Business Types</label
    >
    <div
      class="mt-2 flex gap-4 *:rounded-full *:bg-gray-200 *:px-2 [&_span]:font-bold [&_span]:text-gray-500"
    >
      <p>Physical Store <span>X</span></p>
      <p>Online Store <span>X</span></p>
    </div>
    <form
      action=""
      class="mt-2 flex justify-between rounded-sm border border-gray-500 px-2"
    >
      <input
        type="text"
        name="business_name"
        id="business_name"
        placeholder="Search business types..."
        class="w-full py-2 placeholder-gray-400 outline-none"
      />
      <img
        src={search}
        class="aspect-square w-6"
        alt=""
      />
    </form>
  </div>
</div>
<Footer href="/" textContent="Previous"/>
<Footer href="/forty-one" textContent="Next"/>