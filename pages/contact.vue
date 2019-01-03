<template>
<section class="bg-white">
  <div class="w-full md:w-3/5 container mx-auto px-6 py-8">
    <h1 class="mb-4">Contact</h1>
    <p class="mb-4 leading-normal">You may use the contact form below to email us. We are friendly! :)</p>

    <div class="mb-4">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="sendersName">Name</label>
      <input type="text" class="appearance-none border w-full py-2 px-3 text-grey-darker leading-tight" id="sendersName" name="name" v-model="sendersName">
    </div>
    <div class="mb-4">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="sendersEmail">Email</label>
      <input type="text" class="appearance-none border w-full py-2 px-3 text-grey-darker leading-tight" id="sendersEmail" name="email" v-model="sendersEmail">
    </div>
    <div class="mb-6">
      <label class="block text-grey-darker text-sm font-bold mb-2" for="sendersMessage">Message</label>
      <textarea type="text" class="appearance-none border w-full py-2 px-3 text-grey-darker leading-tight" id="sendersMessage" rows="5" name="message" v-model="sendersMessage"></textarea>
    </div>
    <button class="bg-green hover:bg-green-dark px-8 py-3 text-white text-xl shadow-md border border-green-dark" @click="contactButtonRedirect()">Send Message</button>
  </div>
</section>
</template>