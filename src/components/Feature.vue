<script setup>
    const data = [
        {
        title: "Access your files from anywhere",
        description: "The ability to use a smartphone, tablet, or computer to access your account means your files follow you everywhere.",
        img: "/src/assets/icon-access-anywhere.svg"
        },
        {
        title: "Security you can trust",
        description: "2-factor authentication and user-controlled encryption are just a couple of the security features we allow to help secure your files.",
        img: "/src/assets/icon-security.svg"
        },
        {
        title: "Real-time collaboration",
        description: "Securely share files and folders with friends, family, and colleagues for live collaboration.",
        img: "/src/assets/icon-collaboration.svg"
        },
        {
        title: "Any file, anywhere",
        description: "Upload any type of file, regardless of size, and access it from any device at any time.",
        img: "/src/assets/icon-any-file.svg"
        }
    ]
</script>

<template>
    <section class="features-section features-grid ">
        <div class="features-container feature-card " v-for="value in data">
            <img :src="value.img" :alt="value.title" class="feature-icon-wrapper">
            <h2 class="feature-title">{{ value.title }}</h2>
            <p class="feature-description">{{ value.description }}</p>
        </div>
    </section>
</template>