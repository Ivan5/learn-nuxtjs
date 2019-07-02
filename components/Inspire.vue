<template>
  <h4 class="subtitle">
    <i>"{{ quote }}" - {{ author }}</i>
  </h4>
</template>

<script>
export default {
  data() {
    return {
      quotes: [
        {
          quote: "Life dosen't give you purpose. You give life porpuse",
          author: "The flash"
        },
        {
          quote:
            "Sometimes, to do what's right, we have to give up the things we want the most, Even our dreams",
          author: "Spider-Man"
        },
        {
          quote: "Why do we fall? So that we can learn to pick ourseleves up",
          author: "Alfred"
        },
        {
          quote: "I would rather be a brainless monkey than a heartless moster",
          author: "Goku"
        }
      ],
      quote: "",
      author: ""
    };
  },
  created() {
    let index = Math.floor(Math.random() * this.quotes.length);
    this.quote = this.quotes[index].quote;
    this.author = this.quotes[index].author;
  }
};
</script>

<style>
</style>
