<script lang=ts>
    import { Avatar } from '@skeletonlabs/skeleton';

    let id: number;
    let image: string;
    let title: string;


    let items = [
    { id: 1, title: "Visión General", image: "https://picsum.photos/800/800" },
    { id: 2, title: "Descripción General", image: "https://picsum.photos/800/800" },
    { id: 3, title: "Estudios", image: "https://picsum.photos/800/800" },
    { id: 4, title: "Viabilidad Financiera", image: "https://picsum.photos/800/800" },
    { id: 5, title: "Regulación", image: "https://picsum.photos/800/800" },
    { id: 6, title: "Apoyo banca internacional", image: "https://picsum.photos/800/800" },
    { id: 7, title: "Hitos", image: "https://picsum.photos/800/800" },
    ];
</script>


<div class="w-full bg-slate-500 py-16">
    <div class="container mx-auto">
        <div class="flex items-center justify-center gap-x-32 gap-y-16 flex-wrap">
           {#each items as item (item.id)}
            <a href="#">
                <Avatar src={item.image} alt={item.title} class=" mx-auto w-32 h-32" border="border-4  border-surface hover:!border-primary-500"
                cursor="cursor-pointer"/>
            <h3 class=" h3 text-center p-4">{item.title}</h3>
            </a>
            {/each}
        </div>
       
    </div>



</div>


