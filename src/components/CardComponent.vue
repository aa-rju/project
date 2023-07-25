<template>
      <vs-card type="5">
    <template #title>
      <h3>Pot with a plant</h3>
    </template>
    <template #img>
      <img src="https://media.istockphoto.com/id/1325763688/photo/web-design-development-design-studio-creative-process-3d-render.jpg?s=1024x1024&w=is&k=20&c=umip8GcmcGJyR5rZpfga9XM_W_LLnARuV0Cf-D37O0Q=" alt="">
    </template>
    <template #text>
      <p>
        Lorem ipsum dolor sit amet consectetur, adipisicing elit.
      </p>
    </template>
    <template #interactions>
      <vs-button danger icon>
        <i class='bx bx-heart'></i>
      </vs-button>
      <vs-button class="btn-chat" shadow primary>
        <i class='bx bx-chat' ></i>
        <span class="span">
          54
        </span>
      </vs-button>
    </template>
  </vs-card>

</template>

<script>
export default {
  // ...
  mounted() {
    window.addEventListener('scroll', this.handleScroll);
  },
  destroyed() {
    window.removeEventListener('scroll', this.handleScroll);
  },
  methods: {
    handleScroll() {
      const cards = document.querySelectorAll('.card-animation-scroll');
      cards.forEach((card) => {
        const cardPosition = card.getBoundingClientRect().top;
        const screenHeight = window.innerHeight;
        if (cardPosition < screenHeight) {
          card.classList.add('animate');
        }
      });
    },
  },
};
</script>