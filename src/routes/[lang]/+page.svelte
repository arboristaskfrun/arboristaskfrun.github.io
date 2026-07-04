<script>
  import { Earth, AtSign, PhoneCall, Trees } from "lucide-svelte";
  import Footer from "$lib/Footer.svelte";

  const style = {
    wrapper: "max-w-[1400px] mx-auto px-4 lg:px-6",
    logo: "w-28",
  };
</script>

<nav class=" py-4 h-[102px]">
  <div class="{style.wrapper} flex justify-between items-center">
    <div>
      <img
        class={style.logo}
        width="112"
        height="70"
        src="images/Arborist Askfrun.svg"
        alt="Arborist Askfrun"
      />
    </div>
    <ul class="flex justify-between gap-4 items-center">
      <li>
        <a
          href="/"
          class="flex gap-1.5 items-center px-2 py-1.5 bg-gray-200 rounded-md hover:bg-[var(--color-bg)]"
          ><Earth size={18} /> <span class="pt-1">SE</span></a
        >
      </li>
    </ul>
  </div>
</nav>
<div class="flex flex-col min-h-screen pb-14">
  <main>
    <div class="bg-[#051208] text-emerald-50 overflow-hidden relative">
      <div class="flex flex-col lg:flex-row gap-4 lg:gap-6">
        <div class="h-96 lg:h-auto lg:w-1/2 relative">
          <img
            class="h-full object-cover block absolute top-0 left-0 w-full"
            src="images/arboristaskfrun-top.jpeg"
            alt=""
          />
        </div>
        <div class="px-4 lg:w-1/2 my-6 lg:py-20">
          <h1
            class="text-5xl md:text-6xl tracking-wide my-4 md:py-6 lg:my-9 text-[#f7fffa]"
          >
            Professional tree care for a more beautiful and safer environment
          </h1>
          <p class="md:text-2xl italic font-medium !leading-relaxed">
            Based in the Stockholm area with a wide service range.
          </p>
          <ul class="my-4 md:py-6 lg:my-9 flex gap-4">
            <li>
              <a href="tel:+460720115377" class="button"
                ><PhoneCall /> Phone Number</a
              >
            </li>
            <li>
              <a href="mailto:arborist.askfrun@gmail.com" class="button"
                ><AtSign /> Email</a
              >
            </li>
          </ul>
        </div>
      </div>
    </div>

    <div class="py-6 md:py-11 lg:py-20">
      <div class="px-4 md:text-center md:max-w-3xl mx-auto">
        <h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
          Services
        </h2>
        <ul
          class="font-medium !leading-relaxed flex gap-1.5 md:gap-2 xl:gap-4 flex-wrap md:justify-center text-lg md:text-xl xl:text-2xl"
        >
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]"
          >
            <Trees /> Pruning
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]"
          >
            <Trees /> Advanced tree felling
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]"
          >
            <Trees /> Tree Care Plans & Consultation
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]"
          >
            <Trees /> Planting
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]"
          >
            <Trees /> Risk Assessment
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]"
          >
            <Trees /> Relocation
          </li>
        </ul>
      </div>
    </div>

    <div class="py-6 md:py-11 lg:py-20">
      <div class="px-4 md:text-center md:max-w-3xl mx-auto">
        <h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
          Pris & Trygghet
        </h2>

        <p>• RUT deduction eligible.</p>

        <p>• Trained at Hvilan KY Arborist: completed 2023.</p>

        <p>
          • Liability insurance for property and personal injury with IF with
          insurance number SP5202759.
        </p>

        <p>• Holder of ISA's Tree Risk Assessment Qualification.</p>
      </div>
    </div>

    <div
      class="py-6 md:py-11 lg:py-20 bg-[#04240c] text-emerald-50"
      id="kontak"
    >
      <div class="px-4 md:text-center md:max-w-3xl mx-auto">
        <h2
          class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4 text-[var(--color-bg)]"
        >
          Contact
        </h2>
        <ul
          class="md:text-base font-medium !leading-relaxed flex gap-4 md:justify-center"
        >
          <li>
            <a class="button" target="_blank" href="tel:+460720115377">
              <PhoneCall /> Phone Number
            </a>
          </li>

          <li>
            <a
              class="button"
              target="_blank"
              href="mailto:emelie@arboristaskfrun.se"
            >
              <AtSign /> Email
            </a>
          </li>
        </ul>
      </div>
    </div>

    <div class="py-6 md:py-11 lg:py-20" id="info">
      <h2
        class="px-4 md:text-center text-4xl md:text-5xl tracking-wide !leading-normal mb-4"
      >
        Gallery
      </h2>
      <ul class="flex flex-wrap gap-4 mt-6 md:mt-9 px-4">
        <li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
          <img
            class=""
            src="images/arboristaskfrun2.jpeg"
            alt="Arborist Askfrun at work 1"
          />
        </li>
        <li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
          <img
            class=""
            src="images/arboristaskfrun4.jpeg"
            alt="Arborist Askfrun at work 3"
          />
        </li>
        <li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
          <img
            class=""
            src="images/arboristaskfrun5.jpeg"
            alt="Arborist Askfrun at work 5"
          />
        </li>

        <li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
          <img
            class=""
            src="images/arboristaskfrun9.jpeg"
            alt="Arborist Askfrun at work 9"
          />
        </li>
        <li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
          <img
            class=""
            src="images/arboristaskfrun15.jpeg"
            alt="Arborist Askfrun at work 5"
          />
        </li>
        <li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
          <img
            class=""
            src="images/arboristaskfrun11.jpeg"
            alt="Arborist Askfrun at work 11"
          />
        </li>
      </ul>
      <div class="flex justify-center mt-4">
        <img src="images/TRAQ-Cert.png" alt="Services" class="w-[240px]" />
      </div>
    </div>
  </main>
  <Footer />
</div>
