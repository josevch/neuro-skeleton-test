<script>
    import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
</script>

<div class="w-full bg-slate-400 ">
    <div class="flex sm:flex-col md:flex-row gap-8 ">
        <div class="flex-1  ">
            <img src="https://fastly.picsum.photos/id/43/1000/1000.jpg?hmac=Ntt4paJdg6csRI3czzyLupV8R0y8_43J7Y8X-ijHyME" alt="" srcset="">
        </div>
        <div class="flex-1 container self-center">
            <h2 class="h2 text-rose-950 mb-4  uppercase">Compromiso ambiental y social</h2>
            <p class=" text-rose-950 mb-6 text-justify"> Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi voluptates quae fugit libero fugiat cumque illo nostrum culpa, iusto, neque quibusdam totam harum repellendus expedita facilis pariatur soluta quaerat repellat!</p>
            <Accordion>
                <AccordionItem open>
                    <svelte:fragment slot="lead">(icon)</svelte:fragment>
                    <svelte:fragment slot="summary">(summary)</svelte:fragment>
                    <svelte:fragment slot="content">(content)</svelte:fragment>
                </AccordionItem>
                <AccordionItem>
                    <svelte:fragment slot="lead">(icon)</svelte:fragment>
                    <svelte:fragment slot="summary">(summary)</svelte:fragment>
                    <svelte:fragment slot="content">(content)</svelte:fragment>
                </AccordionItem>
                <AccordionItem>
                    <svelte:fragment slot="lead">(icon)</svelte:fragment>
                    <svelte:fragment slot="summary">(summary)</svelte:fragment>
                    <svelte:fragment slot="content">(content)</svelte:fragment>
                </AccordionItem>
            </Accordion>
           
        </div>
    </div>
</div>