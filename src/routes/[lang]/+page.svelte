<script>
  import { page } from "$app/stores";
  import {
    Earth,
    AtSign,
    PhoneCall,
    Trees,
    TriangleAlert,
  } from "lucide-svelte";
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
          class="flex gap-1.5 items-center px-2 py-1.5 bg-gray-200 rounded-md hover:bg-white"
          ><Earth size={18} /> <span class="pt-1">Swedish</span></a
        >
      </li>
    </ul>
  </div>
</nav>
<div class="flex flex-col min-h-screen pb-14">
  <main>
    <div class="bg-[#04240c] text-emerald-50 overflow-hidden relative">
      <div class="flex flex-col lg:flex-row gap-4 lg:gap-6">
        <div class="h-80 lg:h-auto lg:w-1/2 relative">
          <img
            class="h-full object-cover hidden lg:block absolute top-0 left-0 w-full"
            src="images/arboristaskfrun-top.jpeg"
            alt=""
          />

          <img
            class="h-full object-cover w-full lg:hidden"
            src="images/hero-landscape.jpg"
            alt=""
          />
        </div>
        <div class="px-4 lg:w-1/2 my-6">
          <h1 class="text-5xl md:text-6xl tracking-wide my-4 md:py-6 lg:my-9">
            Arborist Askfrun
          </h1>
          <p class="md:text-2xl italic font-medium !leading-relaxed">
            Your friendly neighborhood arborist in Stockholm, I’m here to help
            you with all your tree care needs. With a deep commitment to
            sustainability and years of hands-on experience, I ensure your trees
            stay healthy and beautiful. Whether it’s pruning, planting, disease
            prevention, or emergency care, you can count on me, Arborist
            Askfrun, to treat your trees with the utmost care and expertise.
          </p>
          <p class="md:text-2xl italic font-medium !leading-relaxed my-4">
            Get in touch with me today for friendly and reliable tree services
            in Stockholm.
          </p>

          <ul class="my-4 md:py-6 lg:my-9 flex gap-4">
            <li>
              <a href="tel:+460720115377" class="button"><PhoneCall /> Call</a>
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

    <div class="py-6 md:py-11 lg:py-20 hidden" id="info">
      <div class="px-4 md:text-center md:max-w-3xl mx-auto">
        <h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
          About
        </h2>
        <p class="md:text-2xl italic font-medium !leading-relaxed mt-4 md:mt-6">
          Hello! I'm Emelie, the proud owner of "Arborist Askfrun" Originally
          from the charming town of Umeå, I now call the vibrant city of
          Stockholm my home. My passion for plants has been a lifelong journey,
          and I've dedicated myself to the art and science of arboriculture.
          There's nothing I love more than nurturing trees and helping them
          thrive.
        </p>
        <p class="md:text-2xl italic font-medium !leading-relaxed mt-4 md:mt-6">
          If you're ever in need of an arbonist, I'm here for you. With my
          knowledge and genuine love for all things green, I’m confident that I
          can provide the best care for your trees. Let's work together to make
          your greenery flourish!
        </p>
      </div>

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

    <div class="py-6 md:py-11 lg:py-20 hidden">
      <div class="px-4 md:text-center md:max-w-3xl mx-auto">
        <h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
          Services
        </h2>
        <ul
          class="font-medium !leading-relaxed flex gap-1.5 md:gap-2 xl:gap-4 flex-wrap md:justify-center text-lg md:text-xl xl:text-2xl"
        >
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-white"
          >
            <Trees /> Care
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-white"
          >
            <Trees /> Management
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-white"
          >
            <Trees /> Planting
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-white"
          >
            <Trees /> Pruning
          </li>
          <li
            class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-white"
          >
            <Trees /> Disease prevention
          </li>
        </ul>
      </div>
    </div>

    <div class="py-6 md:py-11 lg:py-20 hidden">
      <div class="px-4 md:text-center md:max-w-3xl mx-auto">
        <h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
          Pricing
        </h2>

        <ul class="font-medium !leading-relaxed text-lg md:text-xl xl:text-2xl">
          <li
            class="flex justify-between gap-1.5 items-center px-4 py-1.5 border-b border-dashed border-yellow-600"
          >
            <span>Hourly rate</span>
            <span>1,000 SEK</span>
          </li>
          <li
            class="flex justify-between gap-1.5 items-center px-4 py-1.5 border-b border-dashed border-yellow-600"
          >
            <span>Whole day</span>
            <span>7,000 SEK</span>
          </li>
          <li
            class="flex justify-between gap-1.5 items-center px-4 py-1.5 border-b border-dashed border-yellow-600"
          >
            <span>Half Day</span>
            <span>4,000 SEK</span>
          </li>
        </ul>

        <div class="p-4 md:p-6 mt-4 md:mt-6">
          <h2 class="flex gap-2 md:justify-center text-lg">Important note:</h2>
          <p>
            04240c All prices are exclusive of VAT & transportation cost (Price
            per KM. 24.3 SEK).
          </p>
          <p>
            The prices listed are estimates. To provide you with the most
            accurate quote, I will need to visit and assess the condition of the
            tree first.
          </p>
        </div>
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
          Contact Emelie
        </h2>
        <ul
          class="md:text-base font-medium !leading-relaxed flex gap-4 md:justify-center"
        >
          <li>
            <a class="button" target="_blank" href="tel:+460720115377">
              <PhoneCall /> Call
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
  </main>
  <Footer />
</div>
