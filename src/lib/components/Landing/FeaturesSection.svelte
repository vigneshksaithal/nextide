<script lang="ts">
    import FeatureCard from './FeatureCard.svelte';

    const features = [
        {
            title: 'Code Diagrams',
            description: 'Visualize your entire code architecture at a glance to understand dependencies and impact.'
        },
        {
            title: 'Flowchart Diffs',
            description: 'Intuitively grasp logic changes with visual diffs that show flow instead of just text.'
        },
        {
            title: 'Faster Reviews',
            description: 'Leverage AI-powered suggestions and a streamlined UI to complete reviews in record time.'
        }
    ];
</script>

<section id="features" class="py-10 sm:py-20">
    <div class="grid items-start gap-12 md:grid-cols-2">
        <div>
            <h2 class="mb-2 max-w-sm text-4xl font-bold leading-tight tracking-[-0.033em] text-white">
                Everything You Need for Effortless Reviews
            </h2>
            <p class="max-w-sm text-base text-gray-400">
                Next IDE provides a suite of tools to streamline your development workflow.
            </p>
        </div>
        <div class="flex flex-col gap-3">
            {#each features as feature, index}
                <FeatureCard index={index + 1} title={feature.title} description={feature.description} />
            {/each}
        </div>
    </div>
</section>

