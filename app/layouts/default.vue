<template>
  <div>
    <header>
      <NuxtLink to="/">DLC Flooring</NuxtLink>
      <nav>
        <NuxtLink to="/services">Services</NuxtLink>
        <NuxtLink to="/contact">Contact</NuxtLink>
      </nav>
    </header>

    <main>
      <slot />
    </main>

    <footer>© {{ new Date().getFullYear() }} DLC Flooring</footer>
  </div>
</template>