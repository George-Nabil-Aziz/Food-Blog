<template>
  <div class="py-5">
    <div class="card-container flex flex-wrap justify-between text-center">
      <div v-for="(card, index) in cards" :key="index" class="w-1/4 p-3">
        <div><img :src="card.image" alt="Food Image" /></div>
        <h2 class="text-xl py-3">{{ card.h2 }}</h2>
        <p>{{ card.text }}</p>
      </div>
    </div>
  </div>
</template>

<script setup>
import image1 from "../assets/sandwich.jpg";
import image2 from "../assets/steak.jpg";
import image3 from "../assets/cherries.jpg";
import image4 from "../assets/wine.jpg";
import image5 from "../assets/popsicle.jpg";
import image6 from "../assets/salmon.jpg";
import image7 from "../assets/sandwich.jpg";
import image8 from "../assets/croissant.jpg";
const cards = [
  {
    image: image1,
    h2: "The Perfect Sandwich, A Real NYC Classic",
    text: "Just some random text, lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    image: image2,
    h2: "Let Me Tell You About This Steak",
    text: "Once again, some random text to lorem lorem lorem lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    image: image3,
    h2: "TCherries, interrupted",
    text: "Lorem ipsum text praesent tincidunt ipsum lipsum. What else? ",
  },
  {
    image: image4,
    h2: "Once Again, Robust Wine and Vegetable Pasta",
    text: "Lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    image: image5,
    h2: "All I Need Is a Popsicle",
    text: "Lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    image: image6,
    h2: "Salmon For Your Skin",
    text: "Salmon For Your Skin",
  },
  {
    image: image7,
    h2: "The Perfect Sandwich, A Real NYC Classic",
    text: "Just some random text, lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
  {
    image: image8,
    h2: "Le French",
    text: "Lorem lorem lorem lorem ipsum text praesent tincidunt ipsum lipsum.",
  },
];
</script>
