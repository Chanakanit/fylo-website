<script setup>
const reviews = [
  {
    quote: "Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.",
    name: "Satish Patel",
    title: "Founder & CEO, Huddle",
    image: "/src/assets/profile-1.jpg"
  },
  {
    quote: "Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.",
    name: "Bruce McKenzie",
    title: "Founder & CEO, Huddle",
    image: "/src/assets/profile-2.jpg"
  },
  {
    quote: "Fylo has improved our team productivity by an order of magnitude. Since making the switch our team has become a well-oiled collaboration machine.",
    name: "Iva Boyd",
    title: "Founder & CEO, Huddle",
    image: "/src/assets/profile-3.jpg"
  }
]
</script>

<template>
    <section class="relative bg-gray-50 dark:bg-darkBlue px-6 md:px-24 gap-12 mx-auto grid grid-cols-1 pb-72 md:grid-cols-3 pt-8">
        <img src="../assets/bg-quotes.png" alt="quote" class="absolute -top-1 left-6  md:-top-3 md:left-24">
        <div class="bg-gray-100 dark:bg-darkBlue-03 p-6" v-for="review in reviews">
            <p class="text-sm mb-4">{{ review.quote }}</p>
            <div class="flex gap-4 items-center">
                <img :src="review.image" alt="profile" class="w-12 h-12 rounded-full">
                <div>
                    <p class="text-sm font-semibold">{{ review.name }}</p>
                    <p class="text-xs">{{ review.title }}</p>
                </div>
            </div>
        </div>
    </section>
</template>