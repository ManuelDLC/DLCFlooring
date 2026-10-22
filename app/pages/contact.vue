<script setup>
const form = ref({ name: '', email: '', message: '' })

function submit() {
  console.log(form.value)
  alert(`Thanks, ${form.value.name}! We'll be in touch.`)
}
</script>

<template>
  <section>
    <h1>Get a Free Estimate</h1>

    <form @submit.prevent="submit">
      <input v-model="form.name" placeholder="Name" required />
      <input v-model="form.email" type="email" placeholder="Email" required />
      <textarea v-model="form.message" placeholder="Tell us about your project" />
      <button type="submit">Send</button>
    </form>
  </section>
</template>