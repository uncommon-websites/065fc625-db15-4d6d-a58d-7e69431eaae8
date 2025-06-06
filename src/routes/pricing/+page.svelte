<script lang="ts">
	// Types
	import type { PageProps } from "./$types";

	// Components
	import Features from "$lib/components/layout/Features.svelte";
	import Testimonials from "$lib/components/layout/Testimonials.svelte";
	import CallToAction from "$lib/components/layout/CallToAction.svelte";
	import Pricing from "$lib/components/layout/Pricing.svelte";

	// Props
	const { data }: PageProps = $props();
</script>

<Pricing />

<Testimonials
  testimonials={[
    {
      name: "Elise Han",
      position: "CEO",
      company: "Memora Health",
      quote:
        "With Donna, I know exactly where projects stand without chasing updates. It’s like invisibly attending every meeting.",
      image: "/generated/elise-han-east-asian-female-executive-office.webp"
    },
    {
      name: "Jacob Tran",
      position: "Cofounder",
      company: "ZeroNorth",
      quote:
        "Donna surfaces problems before they land in my inbox. I’ve cut down weekly check-in time by over 75%.",
      image: "/generated/jacob-tran-vietnamese-male-founder.webp"
    },
    {
      name: "Nina Gold",
      position: "COO",
      company: "Pivotal AI",
      quote:
        "The productivity visibility helps me debug org issues faster—without resorting to time tracking or intrusive surveys.",
      image: "/generated/image-a-professional-headshot-of-a-black-femal.webp"
    }
  ]}
/>

<CallToAction
  title="Lead with clarity while gaining back your time"
  subtitle="Join the exclusive pilot for CEOs and executives—white-glove onboarding included."
  description="Donna connects your calendar, project tools, and comms to show what’s moving, what’s blocked, and where your team’s time is going. Enjoy real-time visibility and decision-ready insights, all with enterprise-grade privacy and zero data retention. Spots are limited; secure your access and reclaim focus each morning."
  imageSrc="/generated/image-a-happy-executive-standing-in-a-bright-m.webp"
  callsToAction={[{
    href: '/apply',
    label: 'Apply to the pilot',
    variant: 'primary',
  }]}
/>

