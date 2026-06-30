<script>
	import { page } from '$app/stores';
	import {
		Earth,
		AtSign,
		PhoneCall,
		Trees,
		TriangleAlert,
	} from 'lucide-svelte';
	import Footer from '$lib/Footer.svelte';

	const style = {
		wrapper: 'max-w-[1400px] mx-auto px-4 lg:px-6',
		logo: 'w-28',
	};
</script>

<nav class="bg-white py-4 h-[102px]">
	<div class="{style.wrapper} flex justify-between items-center">
		<div>
			<img
				class={style.logo}
				width="112"
				height="70"
				src="images/Arborist Askfrun.svg"
				alt="Arborist Askfrun" />
		</div>
		<ul class="flex justify-between gap-4 items-center">
			<li>
				<a
					href="/"
					class="flex gap-1.5 items-center px-2 py-1.5 bg-gray-200 rounded-md hover:bg-[var(--color-bg)]"
					><Earth size={18} /> <span class="pt-1">Swedish</span></a>
			</li>
		</ul>
	</div>
</nav>
<div class="flex flex-col min-h-screen pb-14">
	<main>
		<div
			class="bg-gradient-to-r from-[#283618] to-[#052B0C] text-emerald-50 overflow-hidden relative">
			<div class="flex flex-col lg:flex-row gap-4 lg:gap-6">
				<div class="h-80 lg:h-auto lg:w-1/2 relative">
					<img
						class="h-full object-cover hidden lg:block absolute top-0 left-0 w-full"
						src="images/arboristaskfrun1.jpeg"
						alt="" />

					<img
						class="h-full object-cover w-full lg:hidden"
						src="images/hero-landscape.jpg"
						alt="" />
				</div>
				<div class="px-4 lg:w-1/2 my-6">
					<h1 class="text-6xl md:text-8xl tracking-wide my-4 md:py-6 lg:my-9">
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
							<a
								href="tel:+460720115377"
								class="button"><PhoneCall /> Call</a>
						</li>
						<li>
							<a
								href="mailto:+arborist.askfrun@gmail.com"
								class="button"><AtSign /> Email</a>
						</li>
					</ul>
				</div>
			</div>
		</div>

		<div
			class="py-6 md:py-11 lg:py-20"
			id="info">
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
						alt="Arborist Askfrun at work 1" />
				</li>
				<li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
					<img
						class=""
						src="images/arboristaskfrun3.jpeg"
						alt="Arborist Askfrun at work 2" />
				</li>
				<li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
					<img
						class=""
						src="images/arboristaskfrun4.jpeg"
						alt="Arborist Askfrun at work 3" />
				</li>
				<li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
					<img
						class=""
						src="images/arboristaskfrun5.jpeg"
						alt="Arborist Askfrun at work 4" />
				</li>
				<li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
					<img
						class=""
						src="images/arboristaskfrun6.jpeg"
						alt="Arborist Askfrun at work 5" />
				</li>
				<li class="w-[calc(100%/3-11px)] rounded-xl overflow-hidden">
					<img
						class=""
						src="images/arboristaskfrun7.jpeg"
						alt="Arborist Askfrun at work 6" />
				</li>
			</ul>
		</div>

		<div class="py-6 md:py-11 lg:py-20 bg-white">
			<div class="px-4 md:text-center md:max-w-3xl mx-auto">
				<h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
					Services
				</h2>
				<ul
					class="font-medium !leading-relaxed flex gap-1.5 md:gap-2 xl:gap-4 flex-wrap md:justify-center text-lg md:text-xl xl:text-2xl">
					<li
						class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]">
						<Trees /> Care
					</li>
					<li
						class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]">
						<Trees /> Management
					</li>
					<li
						class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]">
						<Trees /> Planting
					</li>
					<li
						class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]">
						<Trees /> Pruning
					</li>
					<li
						class="flex gap-1.5 items-center border-l-4 border-[var(--color-primary)] px-4 py-1.5 bg-[var(--color-bg)]">
						<Trees /> Disease prevention
					</li>
				</ul>
			</div>
		</div>

		<div class="py-6 md:py-11 lg:py-20">
			<div class="px-4 md:text-center md:max-w-3xl mx-auto">
				<h2 class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4">
					Pricing
				</h2>

				<ul class="font-medium !leading-relaxed text-lg md:text-xl xl:text-2xl">
					<li
						class="flex justify-between gap-1.5 items-center px-4 py-1.5 border-b border-dashed border-yellow-600">
						<span>Hourly rate</span>
						<span>1,000 SEK</span>
					</li>
					<li
						class="flex justify-between gap-1.5 items-center px-4 py-1.5 border-b border-dashed border-yellow-600">
						<span>Whole day</span>
						<span>7,000 SEK</span>
					</li>
					<li
						class="flex justify-between gap-1.5 items-center px-4 py-1.5 border-b border-dashed border-yellow-600">
						<span>Half Day</span>
						<span>4,000 SEK</span>
					</li>
				</ul>

				<div class="p-4 md:p-6 bg-white mt-4 md:mt-6">
					<h2 class="flex gap-2 md:justify-center text-lg">Important note:</h2>
					<p>
						All prices are exclusive of VAT & transportation cost (Price per KM.
						24.3 SEK).
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
			class="py-6 md:py-11 lg:py-20 bg-gradient-to-r from-[#283618] to-[#052B0C] text-emerald-50"
			id="kontak">
			<div class="px-4 md:text-center md:max-w-3xl mx-auto">
				<h2
					class="text-4xl md:text-5xl tracking-wide !leading-normal mb-4 text-[var(--color-bg)]">
					Contact Emelie
				</h2>
				<ul
					class="md:text-2xl font-medium !leading-relaxed flex gap-4 md:justify-center">
					<li>
						<a
							class="button"
							target="_blank"
							href="tel:+460720115377">
							<PhoneCall /> Call
						</a>
					</li>
					<li>
						<a
							class="button group"
							target="_blank"
							href="https://wa.me/+460720115377">
							<svg
								class="group-hover:fill-[var(--color-bg)] inline-block align-baseline ml-1"
								xmlns="http://www.w3.org/2000/svg"
								height="1em"
								viewBox="0 0 448 512"
								><!--! Font Awesome Free 6.4.2 by @fontawesome - https://fontawesome.com License - https://fontawesome.com/license (Commercial License) Copyright 2023 Fonticons, Inc. --><path
									d="M380.9 97.1C339 55.1 283.2 32 223.9 32c-122.4 0-222 99.6-222 222 0 39.1 10.2 77.3 29.6 111L0 480l117.7-30.9c32.4 17.7 68.9 27 106.1 27h.1c122.3 0 224.1-99.6 224.1-222 0-59.3-25.2-115-67.1-157zm-157 341.6c-33.2 0-65.7-8.9-94-25.7l-6.7-4-69.8 18.3L72 359.2l-4.4-7c-18.5-29.4-28.2-63.3-28.2-98.2 0-101.7 82.8-184.5 184.6-184.5 49.3 0 95.6 19.2 130.4 54.1 34.8 34.9 56.2 81.2 56.1 130.5 0 101.8-84.9 184.6-186.6 184.6zm101.2-138.2c-5.5-2.8-32.8-16.2-37.9-18-5.1-1.9-8.8-2.8-12.5 2.8-3.7 5.6-14.3 18-17.6 21.8-3.2 3.7-6.5 4.2-12 1.4-32.6-16.3-54-29.1-75.5-66-5.7-9.8 5.7-9.1 16.3-30.3 1.8-3.7.9-6.9-.5-9.7-1.4-2.8-12.5-30.1-17.1-41.2-4.5-10.8-9.1-9.3-12.5-9.5-3.2-.2-6.9-.2-10.6-.2-3.7 0-9.7 1.4-14.8 6.9-5.1 5.6-19.4 19-19.4 46.3 0 27.3 19.9 53.7 22.6 57.4 2.8 3.7 39.1 59.7 94.8 83.8 35.2 15.2 49 16.5 66.6 13.9 10.7-1.6 32.8-13.4 37.4-26.4 4.6-13 4.6-24.1 3.2-26.4-1.3-2.5-5-3.9-10.5-6.6z" /></svg>
							WA
						</a>
					</li>
					<li>
						<a
							class="button"
							target="_blank"
							href="mailto:+arborist.askfrun@gmail.com">
							<AtSign /> Email
						</a>
					</li>
				</ul>
			</div>
		</div>
	</main>
	<Footer />
</div>
