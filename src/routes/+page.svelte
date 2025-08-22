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
	title="Draft less. Sign more."
	subtitle="Trusted by 40+ Am Law 100 firms and 54,000+ lawyers worldwide to handle 35% more cases while reducing manual effort by 80%."
	centered={false}
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
	mode="light"

	logoUrls={[
		'https://cdn.brandfetch.io/microsoft.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/jpmorgan.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/pwc.com/w/400/h/400/logo',
		'https://cdn.brandfetch.io/kirkland.com/w/400/h/400/logo'
	]}
/>

<Summary
	title="Built for legal excellence"
	text="Legalo transforms complex legal workflows with domain-specific AI models built by former O'Melveny attorneys and DeepMind researchers. We serve Fortune 500 legal departments and Am Law 100 firms who need to handle increasing case volumes without compromising quality or security. Our platform enables lawyers to manage 35% more cases while reducing manual document review by 80%, freeing legal professionals to focus on strategic, high-value work."
/>

<Testimonials
	testimonials={[
		{
			name: "Victoria Martinez",
			position: "General Counsel",
			company: "Apex Financial Group",
			quote:
				"Legalo reduced our contract review time from weeks to hours.",
			image: "/generated/image-a-professional-female-general-counsel-po.webp"
		},
		{
			name: "Robert Chen",
			position: "Senior Partner",
			company: "Sterling & Associates",
			quote:
				"Legalo saved us $2.3M in the first year with 97% faster contract analysis.",
			image: "/generated/image-a-distinguished-male-senior-partner-posi.webp"
		},
		{
			name: "Amanda Foster",
			position: "Chief Legal Officer",
			company: "TechCorp Industries",
			quote:
				"We've eliminated 80% of manual document review while maintaining full compliance.",
			image: "/generated/image-a-confident-female-chief-legal-officer-s.webp"
		}
	]}
/>

<Features
	title="Intelligent legal AI that scales with your practice"
	subtitle="Transform complex legal workflows with domain-specific AI models that understand the nuances of legal work"
	features={[
		{
			title: "Document review automation",
			description: "Reduce manual document review time by 80% with AI models trained specifically for legal analysis and contract examination."
		},
		{
			title: "Enhanced case capacity",
			description: "Handle 35% more cases without increasing headcount by automating repetitive legal tasks and streamlining complex workflows."
		},
		{
			title: "Enterprise-grade security",
			description: "Protect privileged client data with SOC-2 certified architecture, single-tenant deployment, and all files kept within your firm's VPC."
		},
		{
			title: "Domain-specific intelligence",
			description: "Leverage AI models built by former O'Melveny attorneys and DeepMind researchers who understand both legal practice and cutting-edge AI."
		},
		{
			title: "Workflow automation",
			description: "Design and deploy custom AI workflows that adapt to your firm's specific processes and practice areas."
		},
		{
			title: "Global legal research",
			description: "Access comprehensive legal research across 54+ countries with citation-linked answers sourced from primary-law databases."
		}
	]}
/>
<AboutTeaser generating />
<CallToAction
	title="Stop pushing paper. Start practicing law."
	subtitle="Transform your legal practice today"
	description="Legalo helps your legal team handle 35% more cases by reducing manual review time by 80%. Built by former litigators and DeepMind researchers, Legalo is trusted by 40 of the Am Law 100 and runs in a secure, single-tenant environment with full SOC-2 certification."
	imageSrc="/generated/image-a-successful-general-counsel-at-a-modern.webp"
	callsToAction={[
		{
			href: "#demo",
			label: "Book a demo",
			variant: "primary"
		},
		{
			href: "#contact",
			label: "Talk to sales",
			variant: "secondary"
		}
	]}
/>
