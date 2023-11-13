<template>
  <div class="container">
  
    <NuxtLink to="/demo/home" class="">wakaba</NuxtLink>
  <Progress class="my-4" style="height: 75px">
    <ProgressBar
     striped
     animated
     :value="25">
     25%
    </ProgressBar>
  </Progress>
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

   <!-- Button trigger modal -->
  <b-button
    button="primary"
    toggle="modal"
    target="#staticBackdropLive"
  >
    Launch demo modal
  </b-button>
  <!-- Modal -->
  <Modal
    id="staticBackdropLive"
    backdrop="static"
    :keyboard="false"
  >
    <ModalDialog>
      <ModalContent>
        <ModalHeader>
          <ModalTitle>Modal title</ModalTitle>
          <CloseButton disabled dismiss="modal" />
        </ModalHeader>
        <ModalBody>
          <p>
            I will not close if you click outside me. Don't even try to press
            escape key.
          </p>
        </ModalBody>
        <ModalFooter>
          <b-button
            button="secondary"
            dismiss="modal"
          >
            Close
          </b-button>
          <b-button button="primary">
            Understood
          </b-button>
        </ModalFooter>
      </ModalContent>
    </ModalDialog>
  </Modal>
  </div>
</template>