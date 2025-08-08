<!--
@component AboutTeaser
A compelling founder story teaser that builds personal connection and company credibility.
-->
<script lang="ts">
	// Types
	type Founder = {
		name: string;
		role: string;
		image: string;
		quote: string;
	};

	// Components
	import Button from "../ui/Button.svelte";
	import ScrollText from "./sub/ScrollText.svelte";

	// State
	let sectionRef: HTMLElement;

	let props = $props();

	// Data - Winston Weinberg as the primary founder for the story
	const founder: Founder = {
		name: "Winston Weinberg",
		role: "CEO & Co-Founder",
		image: "/generated/image-a-professional-male-ceo-dressed-in-a-tai.webp",
		quote: "After years at O'Melveny, I watched brilliant lawyers spend 60% of their time on document review instead of strategic counsel. That's not why we got into law. Harvey exists because every lawyer deserves to focus on what they do best: solving complex problems that actually matter."
	};
</script>

<section bind:this={sectionRef} {...props}>
	<div class="section-px section-py container mx-auto">
		<div class="relative mx-auto grid max-w-4xl place-items-center gap-16">
			<ScrollText
				class="text-title1 text-center leading-tight"
				text={`"${founder.quote}"`}
			/>

			<!-- Founder Attribution & CTA Section -->
			<div class="grid items-center gap-8">
				<div class="flex items-center justify-center gap-6">
					<img
						src={founder.image}
						alt={founder.name}
						class="size-16 rounded-full object-cover"
					/>
					<div class="text-left">
						<div class="text-callout font-medium">{founder.name}</div>
						<div class="text-caption text-muted-foreground">{founder.role}</div>
						<div class="text-caption text-muted-foreground mt-1">Former Litigation Attorney, O'Melveny</div>
					</div>
					<Button href="/about" variant="primary" size="md" class="ml-8">
						Our story
					</Button>
				</div>
			</div>
		</div>
	</div>
</section>
