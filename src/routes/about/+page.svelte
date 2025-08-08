<script lang="ts">
	// Components
	import CallToAction from "$lib/components/layout/CallToAction.svelte";

	// Icons
	import StakeholderGrid from "$lib/components/layout/StakeholderGrid.svelte";
	import Story from "./Story.svelte";
	import SecondaryHero from "$lib/components/layout/hero-sections/SecondaryHero.svelte";
	import Culture from "$lib/components/layout/Culture.svelte";

	// Constants
	const values = [
		{
			title: "Legal expertise first",
			description: "Founded by lawyers who lived the pain of manual legal work. Every feature is built with deep understanding of legal workflows and the stakes involved."
		},
		{
			title: "Enterprise-grade security",
			description: "SOC 2-certified, single-tenant architecture with data residency controls. Your privileged information never leaves your VPC."
		},
		{
			title: "Domain precision",
			description: "Purpose-built AI models trained specifically for legal work. Not general-purpose tools adapted for law—real solutions for real legal problems."
		},
		{
			title: "Global reach, local precision",
			description: "Operating in 54+ countries with multi-language support and regional data compliance. Scale globally while meeting local requirements."
		},
		{
			title: "Partnership-driven innovation",
			description: "Co-built with leading law firms and enterprises. Strategic alliances with LexisNexis, Microsoft, and foundational model providers."
		},
		{
			title: "Measurable impact",
			description: "97% accuracy on key extractions. 35% more cases handled. 80% reduction in manual effort. Results that matter to your bottom line."
		}
	];
</script>

<SecondaryHero
	title="AI built for legal work"
	subtitle="Serious speed, without compromise"
	imageSrc="/generated/image-a-group-of-four-diverse-legal-profession.webp"
/>

<!-- Story Section -->
<Story
	paragraphs={[
		"Legalo was founded by Winston Weinberg, a former litigator at O'Melveny, and Gabe Pereyra, a research scientist from DeepMind, who both saw firsthand how much of legal work was broken. Winston spent hours buried in repetitive, manual review. Gabe knew AI could handle complexity—but trusted, secure deployment was a must. Together, they built Legalo to make legal work faster, more accurate, and less tedious—starting with the pain points they knew best.",
		"Instead of general-purpose tools that guess at answers, Legalo trains domain-specific models that understand legal nuance. Built in partnership with firms and legal researchers, its workflows adapt to each matter type—from litigation to regulatory. And with a single-tenant, SOC 2–certified deployment model, Legalo answers the data privacy questions that matter most to legal teams. That's why it's trusted by over 40 Am Law 100 firms and embedded throughout Fortune 500 legal departments.",
		"More than 54,000 lawyers now use Legalo to turn complex processes into fast, auditable workflows. General counsels gain visibility, accuracy, and speed—clients get better results. With a global footprint, co-built models for tax and compliance, and deep integrations across the legal tech ecosystem, Legalo is reshaping how legal teams work. Because no one got into law to chase footnotes."
	]}
/>

<!-- Our Culture Section -->
<Culture {values} />

<!-- StakeholderGrid Section -->
<StakeholderGrid
	stakeholderType="team"
	title="Leadership"
	subtitle="Legal expertise meets AI innovation"
	stakeholders={[
		{
			name: "Winston Weinberg",
			position: "CEO & Co-Founder",
			bio: "Winston experienced the frustrations of manual legal work during litigation at O'Melveny, giving him deep insight into where AI can transform legal practice.",
			image: "/generated/image-a-professional-headshot-of-a-business-ex.webp"
		},
		{
			name: "Gabe Pereyra",
			position: "President & Co-Founder",
			bio: "Gabe experienced the cutting-edge of AI research at DeepMind, understanding both the technical possibilities and limitations of AI systems.",
			image: "/generated/image-a-professional-headshot-of-a-business-ex.webp"
		}
	]}
/>

<StakeholderGrid
	stakeholderType="investor"
	title="Backed by the best"
	subtitle="$300M Series D led by Sequoia Capital"
	stakeholders={[
		{
			name: "Sequoia Capital",
			image: "https://cdn.brandfetch.io/sequoiacap.com/w/400/h/400/logo"
		},
		{
			name: "OpenAI Startup Fund",
			image: "https://logo.clearbit.com/openai.com"
		},
		{
			name: "Kleiner Perkins",
			image: "https://logo.clearbit.com/kleinerperkins.com"
		},
		{
			name: "GV (Google Ventures)",
			image: "https://logo.clearbit.com/gv.com"
		},
		{
			name: "Conviction Partners",
			image: "https://logo.clearbit.com/conviction.vc"
		}
	]}
/>

<!-- CTA Section -->
<CallToAction
	title="Ready to transform your legal work?"
	subtitle="Join 54,000+ lawyers already using Legalo"
	description="Experience the power of domain-specific AI built for legal professionals. See how Legalo can help your team handle 35% more cases while reducing manual effort by 80%."
	imageSrc="/generated/image-a-diverse-legal-team-engaged-in-a-lively.webp"
	callsToAction={[
		{
			href: "/",
			label: "Request demo",
			variant: "primary"
		},
		{
			href: "/",
			label: "Talk to sales",
			variant: "secondary"
		}
	]}
/>
