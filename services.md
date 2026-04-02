---
layout: default
title: How I Can Help
---

<section class="section" style="padding-top: calc(var(--header-height) + 2rem);">
<div class="container">
<div class="section-title">
<h1>How I Can Help</h1>
<p style="margin-top: 1rem; color: var(--color-text-muted); max-width: 800px; margin: 1rem auto 0 auto;">
Lorem ipsum dolor sit amet, consectetur adipiscing elit. Sed do eiusmod tempor incididunt ut labore et dolore magna aliqua. Ut enim ad minim veniam, quis nostrud exercitation ullamco laboris nisi ut aliquip.
</p>
</div>

<div x-data="{ 
    currentSlide: 0, 
    totalCards: 8,
    cardsPerSlide: window.innerWidth >= 1024 ? 3 : (window.innerWidth >= 768 ? 2 : 1),
    init() {
        window.addEventListener('resize', () => {
            this.cardsPerSlide = window.innerWidth >= 1024 ? 3 : (window.innerWidth >= 768 ? 2 : 1);
            if (this.currentSlide > this.maxSlide) this.currentSlide = this.maxSlide;
        });
    },
    get maxSlide() {
        return Math.max(0, this.totalCards - this.cardsPerSlide);
    },
    next() { if (this.currentSlide < this.maxSlide) this.currentSlide++; },
    prev() { if (this.currentSlide > 0) this.currentSlide--; },
    goTo(index) { this.currentSlide = index; }
}">
<div class="flip-card-container">
<div class="carousel-track" :style="`transform: translateX(calc(-100% * ${currentSlide} / ${cardsPerSlide}))`">

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"I'm losing leads because we can't reply fast enough."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>Custom automations to instantly acknowledge messages so you never miss an opportunity.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"My business Wi-Fi is spotty and drops consistently."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>Robust Wi-Fi setup and network mapping to eliminate dead zones completely.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"I'm being quoted $50k and don't know if I really need it."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>Honest, straightforward tech consulting and advocacy to prevent you from being upsold.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"I'm worried about getting hacked or a data breach."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>Bank-level security auditing, proactive monitoring, and firewall setup to protect your business.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"Our computers are painfully slow and crash often."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>System diagnostics and preventative maintenance to keep your tech running smoothly.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"If our office server dies, we lose absolutely everything."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>Secure, automated, and encrypted backup solutions so your data is always safe.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"Our digital files and shared folders are a complete mess."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>Clean, intuitive cloud storage reorganization and sharing setups for your team.</p>
</div>
</div>
</div>

<div class="flip-card" x-data="{ isFlipped: false }" :class="{ 'is-flipped': isFlipped }" @click="isFlipped = !isFlipped">
<div class="flip-card-inner">
<div class="flip-card-front">
<h3>Problem:</h3>
<p>"Technology is just frustrating and confusing."</p>
<div class="hint">Click to flip <i class="fas fa-sync-alt" style="margin-left: 4px;"></i></div>
</div>
<div class="flip-card-back">
<h3>How I Can Help:</h3>
<p>A friendly, patient tech partner to guide you without the dense 'geek speak'.</p>
</div>
</div>
</div>

</div>
</div>

<div class="carousel-nav">
<button class="carousel-arrow" aria-label="Previous" @click="prev()" :disabled="currentSlide === 0">
<i class="fas fa-chevron-left"></i>
</button>
<div class="carousel-dots">
<template x-for="i in (maxSlide + 1)">
<button class="carousel-dot" aria-label="Go to slide" :class="{ 'active': currentSlide === (i - 1) }" @click="goTo(i - 1)"></button>
</template>
</div>
<button class="carousel-arrow" aria-label="Next" @click="next()" :disabled="currentSlide === maxSlide">
<i class="fas fa-chevron-right"></i>
</button>
</div>

</div>
</div>
</section>
