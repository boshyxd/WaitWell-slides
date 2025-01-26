---
theme: default
background: https://images.unsplash.com/photo-1538108149393-fbbd81895907?q=80&w=2928&auto=format&fit=crop
class: text-center
highlighter: shiki
lineNumbers: false
transition: slide-left
title: WaitWell
mdc: true
---

# WaitWell {.text-6xl .font-bold .mb-6}

<div class="mt-4">
  <p class="text-2xl text-emerald-300 mb-8 font-semibold">
    Transforming Emergency Department Experiences
  </p>
</div>

<div class="pt-8">
  <button 
    class="px-6 py-3 rounded-full 
    bg-gradient-to-r from-emerald-500/20 to-teal-500/20 
    hover:from-emerald-500/30 hover:to-teal-500/30 
    border border-emerald-500/30 
    transition-all duration-300
    text-white font-medium
    shadow-lg"
    @click="$slidev.nav.next"
  >
    Begin Presentation <carbon:arrow-right class="inline ml-2"/>
  </button>
</div>

<div class="abs-br m-8">
  <a 
    href="https://github.com/MxvsAtv321/ED-Patient-Flow-System" 
    target="_blank" 
    class="text-xl icon-btn opacity-50 !border-none !hover:text-emerald-300 transition duration-300"
  >
    <carbon-logo-github />
  </a>
</div>

<style>
.slidev-layout {
  background-color: #000;
  background-image: linear-gradient(45deg, rgba(0,0,0,0.8), rgba(0,0,0,0.6)), url('https://images.unsplash.com/photo-1538108149393-fbbd81895907?q=80&w=2928&auto=format&fit=crop');
  background-size: cover;
  background-position: center;
}

h1 {
  background: linear-gradient(120deg, #4EC5D4, #146b8c);
  -webkit-background-clip: text;
  background-clip: text;
  -webkit-text-fill-color: transparent;
  -webkit-text-stroke: 2px black;
  filter: drop-shadow(0 2px 8px rgba(0,0,0,0.5));
}

.text-emerald-300 {
  text-shadow: 
    0 0 1px rgba(0,0,0,1),
    0 0 2px rgba(0,0,0,1),
    0 0 3px rgba(0,0,0,1),
    0 0 4px rgba(0,0,0,1),
    0 2px 8px rgba(0,0,0,0.8);
}

button {
  text-shadow: 0 2px 4px rgba(0,0,0,0.5);
  box-shadow: 
    0 4px 6px -1px rgba(0, 0, 0, 0.3),
    0 2px 4px -1px rgba(0, 0, 0, 0.2);
}
</style>

---
layout: two-cols
class: 'items-center'
transition: fade-out
---

# The Emergency Department Challenge

<div class="flex flex-col gap-4">
  <div v-click class="flex items-center gap-3">
    <div class="p-2 rounded-full bg-red-500/10">
      <carbon:warning-alt class="w-5 h-5 text-red-500"/>
    </div>
    <p><span class="font-bold text-red-400">"I hope I'm going to be OK"</span></p>
  </div>

  <div v-click class="flex items-center gap-3">
    <div class="p-2 rounded-full bg-orange-500/10">
      <carbon:time class="w-5 h-5 text-orange-500"/>
    </div>
    <p><span class="font-bold text-orange-400">"When will I be seen?"</span></p>
  </div>

  <div v-click class="flex items-center gap-3">
    <div class="p-2 rounded-full bg-yellow-500/10">
      <carbon:user-follow class="w-5 h-5 text-yellow-500"/>
    </div>
    <p><span class="font-bold text-yellow-400">"When will the doctor be back?"</span></p>
  </div>

  <div v-click class="flex items-center gap-3">
    <div class="p-2 rounded-full bg-blue-500/10">
      <carbon:help class="w-5 h-5 text-blue-500"/>
    </div>
    <p><span class="font-bold text-blue-400">"Where am I in the queue?"</span></p>
  </div>

  <div v-click class="flex items-center gap-3">
    <div class="p-2 rounded-full bg-purple-500/10">
      <carbon:help-filled class="w-5 h-5 text-purple-500"/>
    </div>
    <p><span class="font-bold text-purple-400">"Have I been forgotten?"</span></p>
  </div>

  <div v-click class="flex items-center gap-3">
    <div class="p-2 rounded-full bg-green-500/10">
      <carbon:document-unknown class="w-5 h-5 text-green-500"/>
    </div>
    <p><span class="font-bold text-green-400">"When will my test results come back?"</span></p>
  </div>
</div>

::right::

<div class="ml-4 flex flex-col justify-center h-full">
  <div v-click class="text-4xl font-bold text-center mb-4 leading-tight" style="background: linear-gradient(45deg, #ff6b6b 0%, #4ecdc4 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
    Every Patient's Voice Matters
  </div>
  <div v-click class="text-center text-gray-500 mb-8">
    Real concerns from real patients
  </div>
  <div v-click class="text-2xl font-bold text-center mb-2" style="background: linear-gradient(45deg, #ff6b6b 0%, #4ecdc4 100%); -webkit-background-clip: text; -webkit-text-fill-color: transparent;">
    Anxiety & Uncertainty
  </div>
  <div v-click class="text-center text-gray-500">
    The hidden cost of waiting
  </div>
</div>

---
layout: default
transition: slide-up
---

# Patient Pain Points & Solutions

<div class="grid grid-cols-2 gap-2 -mt-4">
  <!-- Problem 1 -->
  <div v-click class="transform transition-all duration-500">
    <div class="bg-red-500/10 p-1.5 rounded-lg">
      <h3 class="text-xs font-bold mb-0.5">Wait Time Uncertainty</h3>
      <p class="text-xs opacity-75">"When will I be seen? When will the doctor be back?"</p>
      <ul class="text-xs mt-0.5 space-y-0.5 opacity-75 list-none">
        <li>No visibility into queue position</li>
        <li>Unpredictable doctor return times</li>
      </ul>
    </div>
  </div>

  <!-- Solution 1 -->
  <div v-click class="transform transition-all duration-500">
    <div class="bg-green-500/10 p-1.5 rounded-lg">
      <h3 class="text-xs font-bold mb-0.5">Real-Time Status</h3>
      <p class="text-xs opacity-75">Live queue position and wait estimates</p>
      <ul class="text-xs mt-0.5 space-y-0.5 opacity-75 list-none">
        <li>Clear position in queue</li>
        <li>Estimated doctor return times</li>
      </ul>
    </div>
  </div>

  <!-- Problem 2 -->
  <div v-click class="transform transition-all duration-500">
    <div class="bg-red-500/10 p-1.5 rounded-lg">
      <h3 class="text-xs font-bold mb-0.5">Status Confusion</h3>
      <p class="text-xs opacity-75">"Why am I back in the waiting room?"</p>
      <ul class="text-xs mt-0.5 space-y-0.5 opacity-75 list-none">
        <li>Unclear progress tracking</li>
        <li>No visibility into next steps</li>
      </ul>
    </div>
  </div>

  <!-- Solution 2 -->
  <div v-click class="transform transition-all duration-500">
    <div class="bg-green-500/10 p-1.5 rounded-lg">
      <h3 class="text-xs font-bold mb-0.5">Journey Tracking</h3>
      <p class="text-xs opacity-75">Visual progress map of your ED visit</p>
      <ul class="text-xs mt-0.5 space-y-0.5 opacity-75 list-none">
        <li>Clear progress indicators</li>
        <li>Next steps always visible</li>
      </ul>
    </div>
  </div>

  <!-- Problem 3 -->
  <div v-click class="transform transition-all duration-500">
    <div class="bg-red-500/10 p-1.5 rounded-lg">
      <h3 class="text-xs font-bold mb-0.5">Communication Barriers</h3>
      <p class="text-xs opacity-75">"I don't understand what's next."</p>
      <ul class="text-xs mt-0.5 space-y-0.5 opacity-75 list-none">
        <li>Language barriers</li>
        <li>Medical terminology confusion</li>
      </ul>
    </div>
  </div>

  <!-- Solution 3 -->
  <div v-click class="transform transition-all duration-500">
    <div class="bg-green-500/10 p-1.5 rounded-lg">
      <h3 class="text-xs font-bold mb-0.5">AI-Powered Assistant</h3>
      <p class="text-xs opacity-75">24/7 multilingual support and explanations</p>
      <ul class="text-xs mt-0.5 space-y-0.5 opacity-75 list-none">
        <li>Multiple language support</li>
        <li>Plain language explanations</li>
      </ul>
    </div>
  </div>
</div>

<style>
.transform {
  transition: all 500ms ease;
}
.slidev-vclick-hidden {
  transform: translateY(20px);
  opacity: 0;
}
</style>

---
layout: center
class: text-center
transition: slide-up
---

# How WaitWell Works

<div class="grid grid-cols-3 gap-8 mt-8">
  <div class="flex flex-col items-center">
    <div v-click class="mb-4">
      <img src="/qr-scan.svg" class="w-24 h-24" />
    </div>
    <div v-click class="text-center">
      <h3 class="text-xl font-bold mb-2">Scan</h3>
      <p class="text-sm opacity-75">Simple QR code on wristband</p>
    </div>
  </div>

  <div class="flex flex-col items-center">
    <div v-click class="mb-4">
      <carbon:api class="w-24 h-24 text-blue-500" />
    </div>
    <div v-click class="text-center">
      <h3 class="text-xl font-bold mb-2">Connect</h3>
      <p class="text-sm opacity-75">Instant access on any device</p>
    </div>
  </div>

  <div class="flex flex-col items-center">
    <div v-click class="mb-4">
      <carbon:machine-learning-model class="w-24 h-24 text-green-500" />
    </div>
    <div v-click class="text-center">
      <h3 class="text-xl font-bold mb-2">Support</h3>
      <p class="text-sm opacity-75">AI-powered assistance</p>
    </div>
  </div>
</div>

---
layout: center
class: text-center
transition: slide-up
---

# Transforming Emergency Care

<div class="mt-8 space-y-4">
  <div v-click class="transform transition-all duration-500">
    <h3 class="text-2xl font-bold bg-gradient-to-r from-blue-500 to-teal-500 bg-clip-text text-transparent">
      Reduced Anxiety
    </h3>
    <p class="text-lg opacity-75">Through transparency and continuous updates</p>
  </div>

  <div v-click class="transform transition-all duration-500">
    <h3 class="text-2xl font-bold bg-gradient-to-r from-teal-500 to-green-500 bg-clip-text text-transparent">
      Better Communication
    </h3>
    <p class="text-lg opacity-75">Breaking down language and technical barriers</p>
  </div>

  <div v-click class="transform transition-all duration-500">
    <h3 class="text-2xl font-bold bg-gradient-to-r from-green-500 to-blue-500 bg-clip-text text-transparent">
      Enhanced Care
    </h3>
    <p class="text-lg opacity-75">Letting medical staff focus on treatment</p>
  </div>
</div>

<style>
.slidev-vclick-target {
  transition: all 500ms ease;
}

.slidev-vclick-hidden {
  transform: translateY(50%);
  opacity: 0;
}
</style>

---
layout: center
class: text-center
transition: slide-up
background: black
---

<div class="bg-black/30 p-8 rounded-xl backdrop-blur-sm">
  <div v-click>
    <carbon:favorite-filled class="text-red-500 w-16 h-16 mx-auto mb-4" />
    <h1 class="text-3xl font-bold mb-4">Supporting Our Healthcare Heroes</h1>
  </div>
  
  <div v-click class="text-xl text-blue-200 mb-8">
    Built with dedication for emergency department staff worldwide
  </div>
  
  <div v-click class="text-sm opacity-75">
    McHacks 12 • 2025 • IFEM Challenge
  </div>
</div>

<style>
h1 {
  background-image: linear-gradient(45deg, #4EC5D4 10%, #146b8c 50%);
  background-clip: text;
  -webkit-background-clip: text;
  -webkit-text-fill-color: transparent;
}
</style>

---
layout: center
class: text-center
transition: slide-up
background: black
---

# UI/UX Design

<div class="w-full h-[400px] bg-[#1e1e1e] p-4 rounded-lg">
  <iframe
    src="https://www.figma.com/embed?embed_host=share&url=https%3A%2F%2Fwww.figma.com%2Ffile%2FrgkiZXwYWrRom2Jx40xZV7%2FWaitWell-UI%252FUX%3Ftype%3Ddesign%26node-id%3D0-1%26mode%3Ddesign%26t%3DG7Ato37ZnUvauHEP-1&theme=dark"
    class="w-full h-full rounded shadow-2xl border border-gray-800"
    allowfullscreen
  ></iframe>
</div>

<style>
.dark #figma-container {
  background: #1e1e1e;
  border-color: #333;
}
</style>
