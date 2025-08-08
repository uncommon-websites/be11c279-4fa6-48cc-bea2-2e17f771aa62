<script lang="ts">
	// Components
	import Summary from "$lib/components/layout/Summary.svelte";
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import AboutTeaser from "$lib/components/layout/AboutTeaser.svelte";
	import LogoScroller from "$lib/components/layout/LogoScroller.svelte";
	import CustomerCardHero from "$lib/components/layout/hero-sections/CustomerCardHero.svelte";
</script>

<CustomerCardHero
	title="Harvey transforms legal work with domain-specific AI"
	subtitle="Trusted by 40+ Am Law 100 firms and 54,000+ lawyers worldwide to handle 35% more cases while reducing manual effort by 80%."
	centered={true}
	customers={[
		{
			name: "Sarah Chen",
			position: "General Counsel, Fortune 500 Technology Company",
			imageSrc: "/generated/image-a-professional-female-general-counsel-si.webp"
		},
		{
			name: "Michael Rodriguez",
			position: "Senior Partner, Am Law 100 Firm",
			imageSrc: "/generated/image-a-distinguished-male-senior-partner-stan.webp"
		},
		{
			name: "Emily Thompson",
			position: "Chief Legal Officer, Global Financial Services",
			imageSrc: "/generated/image-a-professional-female-lawyer-standing-ne.webp"
		},
		{
			name: "David Park",
			position: "Legal Director, Multinational Corporation",
			imageSrc: "/generated/image-a-confident-male-legal-director-sitting-.webp"
		},
		{
			name: "Jessica Williams",
			position: "General Counsel, Healthcare Enterprise",
			imageSrc: "/generated/image-a-professional-female-chief-legal-office.webp"
		}
	]}
/>
<LogoScroller
	label="Trusted by industry leaders"
	logoUrls={[
		'https://cdn.brandfetch.io/microsoft.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/jpmorgan.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/pwc.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/deloitte.com/w/400/h/400/logo'
	]}
/>

<Summary
	generating
	title="What we do"
	text="Our technology delivers measurable results through secure, adaptable solutions that directly increase productivity and drive growth."
/>

<Testimonials
	generating
	testimonials={[
		{
			name: "Jane Smith",
			position: "CTO",
			company: "Tech Innovations",
			quote:
				"Their cutting-edge automation boosted our productivity by 35%.\nThe intuitive interface reduced training time and improved team adoption.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "John Doe",
			position: "Director of Operations",
			company: "Global Solutions",
			quote:
				"Their robust security protocols gave us confidence in handling sensitive data.\nThe 24/7 support team resolved issues within hours, not days.",
			image: "https://www.unc.mn/image-placeholder.svg"
		},
		{
			name: "Sarah Johnson",
			position: "Product Manager",
			company: "Future Systems",
			quote:
				"The scalable platform grew seamlessly with our business needs.\nTheir customization options allowed us to tailor solutions perfectly to our workflows.",
			image: "https://www.unc.mn/image-placeholder.svg"
		}
	]}
/>

<Features
	generating
	title="Features"
	subtitle="Some features"
	features={[
		{
			title: "Streamlined Workflows",
			description:
				"Automate repetitive tasks and connect systems to improve productivity with our industry-leading 87% time savings."
		},
		{
			title: "Data Analysis",
			description:
				"Extract meaningful insights from your data with powerful analytical tools backed by proprietary AI algorithms that are 3x more accurate than competitors."
		},
		{
			title: "Secure Collaboration",
			description:
				"Work together seamlessly while maintaining strict data privacy standards with our zero-knowledge architecture and military-grade encryption."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction generating />
