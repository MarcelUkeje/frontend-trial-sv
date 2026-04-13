<script>
  import Header from "$lib/components/Header.svelte";
  import Footer from "$lib/components/Footer.svelte";

  import addBlack from "$lib/images/add-black.svg";
  import arrowLeft from "$lib/images/arrow-left.svg";
  import store from "$lib/images/store.svg";
  import location from "$lib/images/location.svg";
  import phone from "$lib/images/phone.svg";
  import deleteIcon from "$lib/images/delete.svg";
  // import search from "@lib/images/search.svg"
</script>

<svelte:head>
  <title>Screen 42</title>
</svelte:head>

<Header skip={true}/>
<div class="main bg-gray-100 px-4 pb-8">
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
    <label for="business_name" class="font-semibold text-gray-500"
      >Business Email Addresses</label
    >
    <p class="text-gray-500 underline">Skip this step</p>
    <div class="mt-2 flex flex-col gap-4 *:rounded-md">
      <div class="flex justify-between bg-gray-100 p-2">
        <p class="text-gray-500">info@coastalcoffee.com</p>
        <img
          src={deleteIcon}
          class="aspect-square w-6"
          alt=""
        />
      </div>
      <div class="flex justify-between bg-gray-100 p-2">
        <p class="text-gray-500">support@coastalcoffee.com</p>
        <img
          src={deleteIcon}
          class="aspect-square w-6"
          alt=""
        />
      </div>
      <input
        type="text"
        name="business_name"
        id="business_name"
        placeholder="Primary Email Address"
        class="flex w-full justify-between rounded-sm border border-gray-500 px-2 py-2 placeholder-gray-400 outline-none"
      />
      <input
        type="text"
        name="business_name"
        id="business_name2"
        placeholder="Alternative Email Address (Optional)"
        class="flex w-full justify-between rounded-sm border border-gray-500 px-2 py-2 placeholder-gray-400 outline-none"
      />
      <div class="flex justify-center gap-2 border py-2">
        <img
          src={addBlack}
          class="aspect-square w-4"
          alt=""
        />
        <p>Add Another Email Address</p>
      </div>
    </div>
  </div>
</div>
<Footer href="/forty-one" textContent="Previous"/>
