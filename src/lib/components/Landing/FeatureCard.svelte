<script lang="ts">
    export let index: number;
    export let title: string;
    export let description: string;
</script>

<article class="pointed-card flex gap-4 p-4">
    <div class="flex h-10 w-10 items-center justify-center text-xl font-bold text-sky-400">
        {index}
    </div>
    <div class="flex flex-col">
        <h3 class="text-lg font-bold text-white">{title}</h3>
        <p class="text-sm text-gray-400">{description}</p>
    </div>
</article>

