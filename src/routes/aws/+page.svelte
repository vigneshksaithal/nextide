<script lang="ts">
	import { onMount } from 'svelte'

	let showModal = $state(false)

	onMount(() => {
		// Ensure dark mode is applied
		document.documentElement.classList.add('dark')

		// Handle Escape key to close modal
		const handleEscape = (e: KeyboardEvent) => {
			if (e.key === 'Escape' && showModal) {
				showModal = false
			}
		}

		window.addEventListener('keydown', handleEscape)

		return () => {
			window.removeEventListener('keydown', handleEscape)
		}
	})

	function openModal() {
		showModal = true
		// Prevent body scroll when modal is open
		document.body.style.overflow = 'hidden'
	}

	function closeModal() {
		showModal = false
		// Restore body scroll when modal is closed
		document.body.style.overflow = ''
	}
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
					onclick={openModal}
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
					Build apps with AI speed, deploy directly to your AWS account, and pay
					only for what you use.
				</h2>
				<button
					onclick={openModal}
					class="mt-4 flex h-12 items-center justify-center rounded-lg bg-violet-600 px-8 text-base font-bold tracking-wide text-white shadow-[0_0_30px_-5px_rgba(91,19,236,0.6)] transition-all hover:scale-105 hover:bg-violet-600/90"
				>
					Start Building Free
				</button>
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
						<p class="text-sm font-medium text-green-500">cost savings</p>
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
						<p class="text-sm font-medium text-gray-500">to connect</p>
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
						<p class="text-sm font-medium text-blue-400">integrations</p>
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
						Own your infrastructure, control your costs, and deploy with ease.
					</p>
				</div>
				<div class="grid grid-cols-1 gap-8 md:grid-cols-2">
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
								Full access to your AWS resources. No platform lock-in—your app
								stays online even if we disappear.
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
								Pay AWS directly with no markup. Get spot pricing and free tiers
								straight from the source.
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
					Ready to get started?
				</h2>
				<p class="max-w-xl text-lg text-gray-300">
					Join developers building on their own AWS infrastructure with
					AI-powered development.
				</p>
				<button
					onclick={openModal}
					class="h-12 rounded-lg bg-white px-8 text-base font-bold text-gray-900 transition-colors hover:bg-gray-200"
				>
					Start Building Now
				</button>
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
						AI-powered development that deploys directly to your AWS account.
					</p>
				</div>
			</div>
			<div
				class="flex flex-col items-center justify-between gap-4 border-t border-white/5 pt-8 md:flex-row"
			>
				<p class="text-sm text-gray-600">
					© 2024 Lovable + AWS Inc. All rights reserved.
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

	<!-- Modal -->
	{#if showModal}
		<div
			class="fixed inset-0 z-100 flex items-center justify-center p-4"
			onclick={(e) => {
				if (e.target === e.currentTarget) {
					closeModal()
				}
			}}
			onkeydown={(e) => {
				if (e.key === 'Escape') {
					closeModal()
				}
			}}
			role="dialog"
			aria-modal="true"
			aria-labelledby="modal-title"
			tabindex="-1"
		>
			<!-- Backdrop -->
			<div
				class="absolute inset-0 bg-black/80 backdrop-blur-sm"
				role="button"
				tabindex="0"
				onclick={closeModal}
				onkeydown={(e) => {
					if (e.key === 'Enter' || e.key === ' ') {
						closeModal()
					}
				}}
				aria-label="Close modal"
			></div>

			<!-- Modal Content -->
			<div
				class="relative z-10 w-full max-w-2xl rounded-xl border border-white/10 bg-gray-900 shadow-2xl"
			>
				<!-- Close Button -->
				<button
					onclick={closeModal}
					class="absolute right-4 top-4 z-20 flex size-8 items-center justify-center rounded-lg border border-white/10 bg-gray-800 text-gray-400 transition-colors hover:bg-gray-700 hover:text-white"
					aria-label="Close modal"
				>
					<span class="material-symbols-outlined text-lg">close</span>
				</button>

				<!-- Modal Body -->
				<div class="overflow-hidden rounded-xl">
					<iframe
						src="https://tally.so/r/w4g7Zb"
						class="h-[600px] w-full border-0"
						title="Tally Form"
						loading="lazy"
					></iframe>
				</div>
			</div>
		</div>
	{/if}
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
