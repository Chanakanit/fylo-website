<script setup>
import { ref } from 'vue'

const faqs = [
  {
    question: "What is Bookmark?",
    answer: "Lorem ipsum dolor sit amet, consectetur adipiscing elit. Fusce tincidunt justo eget ultricies fringilla. Phasellus blandit ipsum quis quam ornare mattis."
  },
  {
    question: "How can I request a new browser?",
    answer: "Vivamus luctus eros aliquet convallis ultricies. Mauris augue massa, ultricies non ligula. Suspendisse imperdiet."
  },
  {
    question: "Is there a mobile app?",
    answer: "Sed consectetur quam id neque fermentum accumsan. Praesent luctus vestibulum dolor, ut condimentum urna vulputate eget."
  },
  {
    question: "What about other Chromium browsers?",
    answer: "Integer condimentum ipsum id imperdiet finibus. Vivamus in placerat mi, at euismod dui. Aliquam vitae neque eget nisl gravida pellentesque non ut velit."
  },
]

const openIndex = ref(null)
</script>

<template>
  <section class="max-w-3xl mx-auto px-6 py-16 space-y-4">
    <h2 class="text-4xl font-semibold text-center mb-6">
      Frequently Asked Questions
    </h2>
    <p class="text-center mb-6 md:w-3/5 mx-auto">Here are some of our FAQs. If you have any other questions you'd like answered please feel free to email us.</p>
    
    <div class="p-2" v-for="(faq, index) in faqs" :key="index">
      <button 
        @click="openIndex = openIndex === index ? null : index"
        :aria-expanded="openIndex === index"
        class="w-full flex justify-between items-center border-b pb-2 cursor-pointer font-semibold list-none bg-transparent outline-none"
      >
        {{ faq.question }}
        <span 
          class="material-symbols-outlined transition duration-300 ease-in"
          :class="{ 'rotate-x-180': openIndex === index }"
        >
          expand_more
        </span>
      </button>
      
      <p v-show="openIndex === index" class="mt-4 text-slate-800 dark:text-slate-300">
        {{ faq.answer }}
      </p>
    </div>
  </section>
</template>