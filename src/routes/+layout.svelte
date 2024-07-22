<script>
	import '../app.css';
	import { onMount } from 'svelte';
	onMount(() => {
		document.getElementById('isMain')?.classList.remove('loading');
	});
</script>

<svelte:head>
	<title>Arborist Askfrun: Emelie Häggström</title>
	<meta
		name="description"
		content="Stockholm's leading expert in tree care and management. With unparalleled expertise and a commitment to sustainability, Arborist Askfrun ensures your trees remain healthy and beautiful. From pruning and planting to disease prevention and emergency care, trust Arborist Askfrun for all your arboricultural needs. Contact us today for top-tier tree services in Stockholm." />
	<meta
		name="keywords"
		content="Arborist Askfrun, best arborist in Stockholm, tree care Stockholm, tree management Stockholm, professional arborist services, tree pruning Stockholm, tree planting Stockholm, tree disease prevention, emergency tree care Stockholm, top arborist Stockholm, sustainable tree care, expert arborist Stockholm, tree maintenance Stockholm, arboricultural services Stockholm, tree health management" />
	<meta
		name="robots"
		content="index, follow" />
</svelte:head>

<div
	id="isMain"
	class="loading">
	<section class="content">
		<slot />
	</section>
</div>
