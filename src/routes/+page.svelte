<script lang="ts">
    import {
        BackgroundEffects,
        CallToActionSection,
        FeaturesSection,
        FooterSection,
        HeroSection,
        LandingHeader
    } from '$lib';
</script>

<svelte:head>
    <title>Next IDE - The AI Code Reviewer</title>
    <meta
        name="description"
        content="Next IDE provides AI-assisted code reviews, visual diffs, and collaboration tools to accelerate your workflow."
    />
</svelte:head>

<div class="relative flex min-h-screen flex-col overflow-x-hidden bg-[#0D0D0F] text-white">
    <BackgroundEffects />

    <div class="flex flex-1 flex-col">
        <div class="flex justify-center px-4 sm:px-10 md:px-20 lg:px-40">
            <div class="w-full max-w-6xl">
                <LandingHeader />
            </div>
        </div>

        <main class="flex-1">
            <div class="flex justify-center px-4 sm:px-10 md:px-20 lg:px-40">
                <div class="w-full max-w-6xl">
                    <HeroSection />
                    <FeaturesSection />
                    <CallToActionSection />
                </div>
            </div>
        </main>

        <div class="flex justify-center px-4 sm:px-10 md:px-20 lg:px-40">
            <div class="w-full max-w-6xl">
                <FooterSection />
            </div>
        </div>
    </div>
</div>
