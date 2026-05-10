<script setup></script>
<template>
  <footer class="bg-darkBlue-02 py-8 px-6 text-gray-300 lg:px-24">
    <div class="flex flex-col gap-18 md:flex-row justify-between">
        
        <div class="md:col-span-2 flex flex-col space-y-4">
          <div class="flex items-center space-x-4">
            <img src="../assets/icon-phone.svg" alt="phone icon" class="w-4 h-4 shrink-0" />
            <span>+1-543-123-4567</span>
          </div>
          <div class="flex items-center space-x-4">
            <img src="../assets/icon-email.svg" alt="email icon" class="w-4 h-4 shrink-0" />
            <span>example@fylo.com</span>
          </div>
        </div>
        <div class="flex flex-col md:flex-row gap-16 md:gap">
            <div class="flex flex-col space-y-4">
              <a href="#" class="hover:text-accent-cyan">About</a>
              <a href="#" class="hover:text-accent-cyan">Jobs</a>
              <a href="#" class="hover:text-accent-cyan">Press</a>
              <a href="#" class="hover:text-accent-cyan">Blog</a>
            </div>
    
            <div class="flex flex-col space-y-4">
              <a href="#" class="hover:text-accent-cyan">Contact Us</a>
              <a href="#" class="hover:text-accent-cyan">Terms</a>
              <a href="#" class="hover:text-accent-cyan">Privacy</a>
            </div>
        </div>
        <div class="flex justify-center md:justify-start space-x-4">
          <a href="#" aria-label="Facebook" class="w-8 h-8 rounded-full flex items-center justify-center">
            <img src="../assets/facebook.svg" alt="Facebook">
          </a>
          <a href="#" aria-label="Twitter" class="w-8 h-8 rounded-full flex items-center justify-center">
            <img src="../assets/twitter.svg" alt="Twitter">
          </a>
          <a href="#" aria-label="Instagram" class="w-8 h-8 rounded-full flex items-center justify-center">
            <img src="../assets/instagram.svg" alt="Instagram">
          </a>
        </div>
    </div>
  </footer>
</template>