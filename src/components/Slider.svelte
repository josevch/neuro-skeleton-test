<!-- src/Slider.svelte -->
<script>
    let currentSlide = 0;
  
    const slides = [
      'https://picsum.photos/id/13/1920/1080', 
      'https://picsum.photos/id/15/1920/1080',
      'https://picsum.photos/id/11/1920/1080'
    ];
  
    function nextSlide() {
    currentSlide = (currentSlide + 1) % slides.length;
  }

  function prevSlide() {
    currentSlide = (currentSlide - 1 + slides.length) % slides.length;
  }

  function goToSlide(index) {
    currentSlide = index;
  }
  </script>
  
  <div class="slider w-full relative overflow-hidden">
    <div class="flex transition-transform duration-300 ease-in" style="transform: translateX(-{currentSlide * 100}%)">
      {#each slides as slide, index (slide)}
        <div class=" shrink-0 w-full">
          <img class=" w-max h-auto" src={slide} alt={`Slide ${index}`} />
        </div>
      {/each}
    </div>
    <div class=" justify-center absolute bottom-4 left-1/2 transform -translate-x-1/2 flex space-x-2">
      {#each slides as slide, index (slide)}
        <div
          class="dot transition-bg duration-300 ease-in h-3 w-3 rounded-full cursor-pointer bg-gray-500 hover:bg-gray-700"
          class:selected="{index === currentSlide}"
          on:click="{() => goToSlide(index)}"
        ></div>
      {/each}
    </div>
    <div class=" text-xl left absolute top-1/2 left-4 transform -translate-y-1/2" on:click="{prevSlide}">&larr;</div>
    <div class=" text-xl right absolute top-1/2 right-4 transform -translate-y-1/2" on:click="{nextSlide}">&rarr;</div>
  </div>
