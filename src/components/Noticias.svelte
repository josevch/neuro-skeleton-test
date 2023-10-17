<!-- src/News.svelte -->
<script>
    let news = [
      {
        title: 'Noticia 1',
        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolor sequi nihil est fugiat blanditiis. Fugit quod alias repellendus labore ad odit modi vero, mollitia, aliquam accusamus necessitatibus voluptatibus laudantium.',
        image: 'https://picsum.photos/600/300' // Add image file name or URL here
      },
      {
        title: 'Noticia 2',
        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolor sequi nihil est fugiat blanditiis. Fugit quod alias repellendus labore ad odit modi vero, mollitia, aliquam accusamus necessitatibus voluptatibus laudantium.',
        image: 'https://picsum.photos/600/300' // Add image file name or URL here
      },
      {
        title: 'Noticia 3',
        content: 'Lorem ipsum dolor sit amet consectetur adipisicing elit. Nisi dolor sequi nihil est fugiat blanditiis. Fugit quod alias repellendus labore ad odit modi vero, mollitia, aliquam accusamus necessitatibus voluptatibus laudantium.',
        image: 'https://picsum.photos/600/300' // Add image file name or URL here
      }
    ];
  </script>
  

  <section class="container py-16 mx-auto">
    {#each news as item (item.title)}
      <div class="flex flex-col sm:flex-row gap-4 p-2 items-center justify-left ">
        <div class="image flex-1 w-full">
          <img src={item.image} alt={item.title} class="rounded-xl" />
        </div>
        <div class="info flex-1">
          <h2 class="h2">{item.title}</h2>
          <p>{item.content}</p>
        </div>
      </div>
    {/each}
  </section>
  
