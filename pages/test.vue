<template>
  <div class="container">
    <NuxtLink to="/demo/home" class="">wakaba</NuxtLink>
  <Carousel
    control
    dark
  >
    <CarouselInner>
      <CarouselItem interval="0">
        <CarouselItemImage
          width="800"
          src="https://source.unsplash.com/random/1920x1080?sig=1"
        />
      </CarouselItem>
      <CarouselItem interval="1">
        <CarouselItemImage
          width="800"
          src="https://source.unsplash.com/random/1920x1080?sig=2"
        />
      </CarouselItem>
      <CarouselItem interval="1">
        <CarouselItemImage
          width="800"
          src="https://source.unsplash.com/random/1920x1080?sig=3"
        />
      </CarouselItem>
    </CarouselInner>
  </Carousel>

  
  </div>
</template>