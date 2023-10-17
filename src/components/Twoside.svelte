<script>
    import { Accordion, AccordionItem } from '@skeletonlabs/skeleton';
</script>

<div class="w-full bg-slate-400 ">
    <div class="flex flex-col md:flex-row gap-8 ">
        <div class="flex-1   ">
            <img src="https://fastly.picsum.photos/id/43/1000/1000.jpg?hmac=Ntt4paJdg6csRI3czzyLupV8R0y8_43J7Y8X-ijHyME" alt="" srcset="" class="w-full h-full">
        </div>
        <div class="flex-1 self-center  p-8 ">
            <h2 class="h2 text-rose-950 mb-4  uppercase">Compromiso ambiental y social</h2>
            <p class=" text-rose-950 mb-6 text-justify"> Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi voluptates quae fugit libero fugiat cumque illo nostrum culpa, iusto, neque quibusdam totam harum repellendus expedita facilis pariatur soluta quaerat repellat!</p>
            <Accordion >
                <AccordionItem class="accordion w-full space-y-1 card p-4 text-token rounded-sm " >
                    <svelte:fragment slot="summary" >Estudios</svelte:fragment>
                    <svelte:fragment slot="content">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolor sequi nihil est fugiat blanditiis. Fugit quod alias repellendus labore ad odit modi vero, mollitia, aliquam accusamus necessitatibus voluptatibus laudantium</svelte:fragment>
                </AccordionItem>
                <AccordionItem class="accordion w-full space-y-1 card p-4 text-token rounded-sm" >
                  
                    <svelte:fragment slot="summary">Diseños</svelte:fragment>
                    <svelte:fragment slot="content">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolor sequi nihil est fugiat blanditiis. Fugit quod alias repellendus labore ad odit modi vero, mollitia, aliquam accusamus necessitatibus voluptatibus laudantium</svelte:fragment>
                </AccordionItem>
                <AccordionItem class="accordion w-full space-y-1 card p-4 text-token rounded-sm" >
                  
                    <svelte:fragment slot="summary">Consultas previas</svelte:fragment>
                    <svelte:fragment slot="content">Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolor sequi nihil est fugiat blanditiis. Fugit quod alias repellendus labore ad odit modi vero, mollitia, aliquam accusamus necessitatibus voluptatibus laudantium</svelte:fragment>
                </AccordionItem>
            </Accordion>
           
        </div>
    </div>
</div>