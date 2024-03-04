<script>
    import ProductCard from "./ProductCard.svelte";
    import SectionWrapper from "./SectionWrapper.svelte";
    let productFeatures = [
        {
            featureList: [
                "Daily streak counter",
                "Weights and reps tracker",
                "Community challenges",
                "Every workout is new and exciting",
            ],
            description: "PowerFit ensures all users have the information they need to train safely and train effectively.",
            imgUrl: "",
        },
        {
            featureList: [
                "Daily streak counter",
                "Weights and reps tracker",
                "Community challenges",
                "Every workout is new and exciting",
            ],
            description: "PowerFit ensures all users have the information they need to train safely and train effectively.",
            imgUrl: "",
        },
        {
            featureList: [
                "Daily streak counter",
                "Weights and reps tracker",
                "Community challenges",
                "Every workout is new and exciting",
            ],
            description: "PowerFit ensures all users have the information they need to train safely and train effectively.",
            imgUrl: "",
        }
    ]
</script>
<SectionWrapper id="project">
    <div class="flex flex-col gap-10 sm:gap-14 md:gap-24 flex-1 items-center justify-center pb-10 md:pb-14">
        <div class="flex flex-col gap-2">
            <p class="opacity-60 text-base sm:text-lg md:text-xl text-center">
                Start your lifetime <span class="text-indigo-400">gym streak</span>
                today
            </p>
            <h3 class="text-4xl sm:text-5xl md:text-6xl max-w-[1000px] mx-auto w-full font-semibold text-center">Features for everyone</h3>
        </div>
        <div class="grid grid-cols-1 md:grid-cols-2 gap-10 md:gap-14 lg:gap-20 w-full relative text-base">
            {#each productFeatures as productFeature, index}
                <ProductCard productFeature={productFeature} index={index}>
                    {#if index === 0}

                    {:else if index === 1}
                    {:else}
                    {/if}
                </ProductCard>
            {/each}
        </div>
    </div>
</SectionWrapper>