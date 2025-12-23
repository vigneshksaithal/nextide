<script lang="ts">
	import { onMount } from 'svelte'

	onMount(() => {
		// Ensure dark mode is applied
		document.documentElement.classList.add('dark')
	})
</script>

<svelte:head>
	<title>Lovable + AWS - Vibe Coding Platform</title>
	<meta
		name="description"
		content="Lovable connects directly to your AWS account. Build apps with AI speed (vibe coding), but pay raw infrastructure prices."
	/>
</svelte:head>

<div class="relative flex min-h-screen w-full flex-col">
	<!-- Header -->
	<header
		class="sticky top-0 z-50 w-full border-b border-white/5 bg-gray-900/80 backdrop-blur-md"
	>
		<div
			class="mx-auto flex w-full max-w-7xl items-center justify-between px-4 py-3 md:px-10"
		>
			<div class="flex items-center gap-4">
				<div class="flex size-8 items-center justify-center text-violet-600">
					<span class="material-symbols-outlined text-3xl">all_inclusive</span>
				</div>
				<h2 class="text-lg font-bold tracking-tight text-white">
					Lovable + AWS
				</h2>
			</div>
			<div class="flex items-center">
				<button
					class="rounded-lg bg-violet-600 px-4 py-2 text-sm font-semibold text-white shadow-[0_0_15px_-5px_rgba(91,19,236,0.6)] transition-colors hover:bg-violet-600/90"
				>
					Join Now
				</button>
			</div>
		</div>
	</header>

	<!-- Main Content -->
	<main class="flex flex-1 flex-col items-center w-full">
		<!-- Hero Section -->
		<section
			class="relative flex w-full justify-center overflow-hidden px-4 py-12 md:py-24"
		>
			<div
				class="pointer-events-none absolute left-1/2 top-0 z-0 h-[600px] w-[1000px] -translate-x-1/2 bg-hero-glow"
			></div>
			<div
				class="relative z-10 flex w-full max-w-7xl flex-col items-center gap-8 text-center"
			>
				<h1
					class="max-w-4xl bg-gradient-to-b from-white to-white/60 bg-clip-text text-5xl font-black leading-[1.1] tracking-tight text-transparent md:text-7xl"
				>
					Your Code. Your Cloud. <br />
					<span class="text-violet-600">Zero Markup.</span>
				</h1>
				<h2
					class="max-w-2xl text-lg font-normal leading-relaxed text-gray-400 md:text-xl"
				>
					Lovable connects directly to your AWS account. Build apps with AI
					speed (vibe coding), but pay raw infrastructure prices. Stop renting
					your own success.
				</h2>
				<div class="mt-4 flex w-full flex-wrap justify-center gap-4 sm:w-auto">
					<button
						class="flex h-12 items-center justify-center rounded-lg bg-violet-600 px-8 text-base font-bold tracking-wide text-white shadow-[0_0_30px_-5px_rgba(91,19,236,0.6)] transition-all hover:scale-105 hover:bg-violet-600/90"
					>
						Start Building Free
					</button>
					<button
						class="group flex h-12 items-center justify-center rounded-lg border border-white/10 bg-gray-800 px-8 text-base font-bold text-white transition-all hover:border-white/20 hover:bg-gray-800/80"
					>
						View Documentation
						<span
							class="ml-2 text-sm transition-transform group-hover:translate-x-1 material-symbols-outlined"
							>arrow_forward</span
						>
					</button>
				</div>
				<div
					class="group mt-16 w-full max-w-5xl overflow-hidden rounded-xl border border-white/10 bg-[#0d0b14] shadow-2xl"
				>
					<div
						class="flex items-center gap-2 border-b border-white/5 bg-[#1a1625] px-4 py-3"
					>
						<div class="flex gap-2">
							<div class="size-3 rounded-full bg-red-500/80"></div>
							<div class="size-3 rounded-full bg-yellow-500/80"></div>
							<div class="size-3 rounded-full bg-green-500/80"></div>
						</div>
						<div class="ml-4 font-mono text-xs text-gray-500">
							deploy-pipeline.sh
						</div>
					</div>
					<div class="grid md:grid-cols-2">
						<div
							class="border-b border-white/5 bg-[#0d0b14] p-6 font-mono text-sm text-gray-300 md:border-b-0 md:border-r md:p-8"
						>
							<p class="mb-2 text-gray-500"># Describe your app layout</p>
							<p class="mb-4 text-violet-600">
								Prompt: "Create a dashboard with a sidebar navigation, a
								real-time revenue chart using Recharts, and a user settings form
								connected to DynamoDB."
							</p>
							<p class="text-green-400 typing-effect">
								&gt; Analyzing requirements...
							</p>
							<p class="text-green-400">
								&gt; Generating Next.js components...
							</p>
							<p class="text-green-400">
								&gt; Configuring AWS CloudFormation...
							</p>
						</div>
						<div
							class="relative flex min-h-[300px] items-center justify-center bg-[#110e18] p-4"
						>
							<div
								class="absolute inset-0 bg-cover bg-center opacity-30 mix-blend-overlay"
								style="background-image: url('https://lh3.googleusercontent.com/aida-public/AB6AXuA0Pm6P3QHnwV46qIAXB36a-pJzcOs_dMc-_5045nLhwaCXe_gWwN__kYLHLsrophsiRVyJze0O3zno1i9FCW0pXEZlHQ3kGtWG5WHCQIffJP4vUR3pKJwVVnzj0lCq3KVAozWLnhL3L579CjWY4w8bq1yE3wjXCBIyMZmPO1MXZn0x7Yw6_4PTa3ZRYy60XITbs8eWLM1IUCyDg1mTAdxLY7-fUPULpOriIApg2Z-_1o-6fSVvtloTa8T-S6NyT602jesimKhzVLEE')"
							></div>
							<div class="relative z-10 flex w-full max-w-xs flex-col gap-4">
								<div
									class="flex items-center justify-between rounded border border-violet-600/30 bg-gray-800 p-3 shadow-[0_0_15px_-5px_rgba(91,19,236,0.3)]"
								>
									<div class="flex items-center gap-3">
										<span class="material-symbols-outlined text-violet-600"
											>cloud_queue</span
										>
										<span class="text-sm font-medium text-white"
											>AWS Account</span
										>
									</div>
									<span class="text-xs text-green-400">Connected</span>
								</div>
								<div class="h-8 w-px self-center bg-white/10"></div>
								<div class="grid grid-cols-3 gap-2">
									<div
										class="flex flex-col items-center gap-1 rounded border border-white/5 bg-white/5 p-2"
									>
										<span
											class="material-symbols-outlined text-xs text-blue-400"
											>storage</span
										>
										<span class="text-[10px] text-gray-400">S3</span>
									</div>
									<div
										class="flex flex-col items-center gap-1 rounded border border-white/5 bg-white/5 p-2"
									>
										<span
											class="material-symbols-outlined text-xs text-orange-400"
											>functions</span
										>
										<span class="text-[10px] text-gray-400">Lambda</span>
									</div>
									<div
										class="flex flex-col items-center gap-1 rounded border border-white/5 bg-white/5 p-2"
									>
										<span
											class="material-symbols-outlined text-xs text-purple-400"
											>table_chart</span
										>
										<span class="text-[10px] text-gray-400">Dynamo</span>
									</div>
								</div>
							</div>
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- Stats Section -->
		<section
			class="flex w-full justify-center border-y border-white/5 bg-gray-800/30 px-4 py-10"
		>
			<div class="grid w-full max-w-6xl grid-cols-1 gap-6 md:grid-cols-3">
				<div
					class="flex flex-col gap-2 rounded-xl border border-white/5 bg-gray-800 p-6 transition-colors hover:border-violet-600/20"
				>
					<div class="flex items-start justify-between">
						<p
							class="text-sm font-medium uppercase tracking-wide text-gray-400"
						>
							Average Savings
						</p>
						<span class="material-symbols-outlined text-green-500"
							>trending_down</span
						>
					</div>
					<div class="flex items-baseline gap-2">
						<p class="text-4xl font-bold tracking-tight text-white">60%</p>
						<p class="text-sm font-medium text-green-500">vs Managed PaaS</p>
					</div>
				</div>
				<div
					class="flex flex-col gap-2 rounded-xl border border-white/5 bg-gray-800 p-6 transition-colors hover:border-violet-600/20"
				>
					<div class="flex items-start justify-between">
						<p
							class="text-sm font-medium uppercase tracking-wide text-gray-400"
						>
							Setup Time
						</p>
						<span class="material-symbols-outlined text-violet-600">timer</span>
					</div>
					<div class="flex items-baseline gap-2">
						<p class="text-4xl font-bold tracking-tight text-white">2 min</p>
						<p class="text-sm font-medium text-gray-500">Connect via IAM</p>
					</div>
				</div>
				<div
					class="flex flex-col gap-2 rounded-xl border border-white/5 bg-gray-800 p-6 transition-colors hover:border-violet-600/20"
				>
					<div class="flex items-start justify-between">
						<p
							class="text-sm font-medium uppercase tracking-wide text-gray-400"
						>
							AWS Services
						</p>
						<span class="material-symbols-outlined text-blue-400">hub</span>
					</div>
					<div class="flex items-baseline gap-2">
						<p class="text-4xl font-bold tracking-tight text-white">20+</p>
						<p class="text-sm font-medium text-blue-400">Natively supported</p>
					</div>
				</div>
			</div>
		</section>

		<!-- Features Section -->
		<section class="flex w-full justify-center px-4 py-24">
			<div class="flex w-full max-w-6xl flex-col gap-16">
				<div class="mx-auto flex max-w-3xl flex-col gap-4 text-center">
					<h2 class="text-3xl font-black tracking-tight text-white md:text-5xl">
						Why Lovable + AWS?
					</h2>
					<p class="text-lg text-gray-400">
						Experience the freedom of owning your infrastructure without the
						complexity of managing it manually. We bridge the gap between
						"Vercel-easy" and "AWS-cheap".
					</p>
				</div>
				<div class="grid grid-cols-1 gap-8 md:grid-cols-3">
					<div
						class="group flex flex-col gap-6 rounded-2xl border border-white/5 bg-gray-800/20 p-6 transition-colors hover:bg-gray-800/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-800 text-white"
						>
							<span class="material-symbols-outlined">vpn_key</span>
						</div>
						<div class="flex flex-col gap-2">
							<h3
								class="text-xl font-bold text-white transition-colors group-hover:text-violet-600"
							>
								Own the Infrastructure
							</h3>
							<p class="text-sm leading-relaxed text-gray-400">
								No platform lock-in. You keep the keys and full access to your
								AWS resources. If we disappear tomorrow, your app stays online.
							</p>
						</div>
					</div>
					<div
						class="group flex flex-col gap-6 rounded-2xl border border-white/5 bg-gray-800/20 p-6 transition-colors hover:bg-gray-800/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-800 text-white"
						>
							<span class="material-symbols-outlined">attach_money</span>
						</div>
						<div class="flex flex-col gap-2">
							<h3
								class="text-xl font-bold text-white transition-colors group-hover:text-violet-600"
							>
								Cost Control
							</h3>
							<p class="text-sm leading-relaxed text-gray-400">
								Pay AWS directly. We don't mark up your bandwidth or compute
								costs. Enjoy the spot pricing and free tiers directly from the
								source.
							</p>
						</div>
					</div>
					<div
						class="group flex flex-col gap-6 rounded-2xl border border-white/5 bg-gray-800/20 p-6 transition-colors hover:bg-gray-800/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-800 text-white"
						>
							<span class="material-symbols-outlined">auto_awesome</span>
						</div>
						<div class="flex flex-col gap-2">
							<h3
								class="text-xl font-bold text-white transition-colors group-hover:text-violet-600"
							>
								Vibe Coding
							</h3>
							<p class="text-sm leading-relaxed text-gray-400">
								Describe your app in plain English, and we deploy the full stack
								instantly. From prompt to production in minutes.
							</p>
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- Technical Precision Section -->
		<section
			class="flex w-full justify-center border-t border-white/5 bg-gray-800/20 px-4 py-24"
		>
			<div class="flex w-full max-w-6xl flex-col gap-12">
				<div class="flex max-w-2xl flex-col gap-4">
					<h2 class="text-3xl font-black tracking-tight text-white md:text-4xl">
						Technical Precision
					</h2>
					<p class="text-base text-gray-400">
						Built for developers who want the speed of a PaaS with the raw power
						of IaaS.
					</p>
				</div>
				<div class="grid grid-cols-1 gap-4 md:grid-cols-2 lg:grid-cols-4">
					<div
						class="flex flex-col gap-4 rounded-xl border border-white/5 bg-gray-800 p-6 transition-all hover:-translate-y-1 hover:border-violet-600/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-900 text-white"
						>
							<span class="material-symbols-outlined">cloud_off</span>
						</div>
						<div>
							<h3 class="mb-1 text-base font-bold text-white">
								Zero Markup Hosting
							</h3>
							<p class="text-sm text-gray-400">
								Deploy static sites and assets without the markup tax. Pay only
								for what you use.
							</p>
						</div>
					</div>
					<div
						class="flex flex-col gap-4 rounded-xl border border-white/5 bg-gray-800 p-6 transition-all hover:-translate-y-1 hover:border-violet-600/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-900 text-white"
						>
							<span class="material-symbols-outlined">database</span>
						</div>
						<div>
							<h3 class="mb-1 text-base font-bold text-white">
								Direct S3 Access
							</h3>
							<p class="text-sm text-gray-400">
								Upload and manage files directly in your own buckets. Full ACL
								control.
							</p>
						</div>
					</div>
					<div
						class="flex flex-col gap-4 rounded-xl border border-white/5 bg-gray-800 p-6 transition-all hover:-translate-y-1 hover:border-violet-600/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-900 text-white"
						>
							<span class="material-symbols-outlined">code</span>
						</div>
						<div>
							<h3 class="mb-1 text-base font-bold text-white">
								Lambda Integration
							</h3>
							<p class="text-sm text-gray-400">
								Serverless functions generated by AI and deployed directly to
								your account.
							</p>
						</div>
					</div>
					<div
						class="flex flex-col gap-4 rounded-xl border border-white/5 bg-gray-800 p-6 transition-all hover:-translate-y-1 hover:border-violet-600/40"
					>
						<div
							class="flex size-12 items-center justify-center rounded-lg border border-white/10 bg-gray-900 text-white"
						>
							<span class="material-symbols-outlined">rocket_launch</span>
						</div>
						<div>
							<h3 class="mb-1 text-base font-bold text-white">
								One-Click Deploy
							</h3>
							<p class="text-sm text-gray-400">
								Push to production in seconds with fully automated CI/CD
								pipelines.
							</p>
						</div>
					</div>
				</div>
			</div>
		</section>

		<!-- CTA Section -->
		<section
			class="flex w-full justify-center bg-gradient-to-b from-gray-900 to-[#241c33] px-4 py-20"
		>
			<div
				class="flex w-full max-w-4xl flex-col items-center gap-8 text-center"
			>
				<h2 class="text-4xl font-black tracking-tight text-white md:text-5xl">
					Ready to stop overpaying?
				</h2>
				<p class="max-w-xl text-lg text-gray-300">
					Join thousands of developers building the future of the web on their
					own infrastructure, with the best developer experience in the world.
				</p>
				<div class="flex w-full flex-col justify-center gap-4 sm:flex-row">
					<button
						class="h-12 rounded-lg bg-white px-8 text-base font-bold text-gray-900 transition-colors hover:bg-gray-200"
					>
						Start Building Now
					</button>
					<button
						class="h-12 rounded-lg border border-white/20 bg-transparent px-8 text-base font-bold text-white transition-colors hover:bg-white/5"
					>
						Contact Sales
					</button>
				</div>
			</div>
		</section>
	</main>

	<!-- Footer -->
	<footer
		class="flex w-full justify-center border-t border-white/10 bg-gray-900 px-4 pb-8 pt-16"
	>
		<div class="flex w-full max-w-7xl flex-col gap-12">
			<div class="flex flex-col gap-8 md:flex-row">
				<div class="flex flex-col gap-4 pr-8">
					<div class="flex items-center gap-2">
						<div
							class="flex size-6 items-center justify-center text-violet-600"
						>
							<span class="material-symbols-outlined text-2xl"
								>all_inclusive</span
							>
						</div>
						<span class="font-bold text-white">Lovable + AWS</span>
					</div>
					<p class="max-w-xs text-sm text-gray-500">
						The modern way to build on AWS. AI-native development environment
						that deploys directly to your cloud account.
					</p>
				</div>
			</div>
			<div
				class="flex flex-col items-center justify-between gap-4 border-t border-white/5 pt-8 md:flex-row"
			>
				<p class="text-sm text-gray-600">
					© 2024 Lovable Labs Inc. All rights reserved.
				</p>
				<div class="flex items-center gap-2">
					<span class="relative flex h-2 w-2">
						<span class="relative inline-flex h-2 w-2 rounded-full bg-green-500"
						></span>
					</span>
					<span class="text-sm text-gray-500">All systems operational</span>
				</div>
			</div>
		</div>
	</footer>
</div>

<style>
	/* Hero glow gradient background */
	:global(.bg-hero-glow) {
		background-image: radial-gradient(
			circle at center,
			rgba(91, 19, 236, 0.15) 0%,
			rgba(22, 16, 34, 0) 70%
		);
	}

	/* Custom scrollbar for dark mode */
	:global(::-webkit-scrollbar) {
		width: 8px;
	}

	:global(::-webkit-scrollbar-track) {
		background: #161022;
	}

	:global(::-webkit-scrollbar-thumb) {
		background: #2e2839;
		border-radius: 4px;
	}

	:global(::-webkit-scrollbar-thumb:hover) {
		background: #5b13ec;
	}

	/* Animation for fade-in-up effect */
	@keyframes fade-in-up {
		from {
			opacity: 0;
			transform: translateY(10px);
		}
		to {
			opacity: 1;
			transform: translateY(0);
		}
	}

	:global(.animate-fade-in-up) {
		animation: fade-in-up 0.6s ease-out;
	}

	/* Typing effect animation */
	@keyframes typing {
		from {
			width: 0;
		}
		to {
			width: 100%;
		}
	}

	:global(.typing-effect) {
		overflow: hidden;
		white-space: nowrap;
		animation: typing 2s steps(40, end);
	}
</style>
