<template>
  <header>
    <h1 id="logo"><router-link to="/">Vue Composition UI</router-link></h1>

    <div id="links">
      <img src="https://img.shields.io/badge/PRs-welcome-brightgreen" />
      <template v-for="link of links" :key="link.href">
        <a :href="link.href" :target="link.target">{{ link.label }}</a>
      </template>
    </div>
  </header>
</template>

<script lang="ts">
import { defineComponent } from 'vue'

export default defineComponent({
  name: 'Header',

  setup() {
    const links = [
      {
        label: 'API reference',
        href: 'https://github.com/js-cosmos/vue-composition-ui/blob/HEAD/api-reference/index.md',
        target: '_blank',
      },
      {
        label: 'GitHub',
        href: 'https://github.com/js-cosmos/vue-composition-ui',
        target: '_blank',
      },
    ]
    return {
      links,
    }
  },
})
</script>

<style scoped>
header {
  display: grid;
  grid-template-columns: 250px auto;
  grid-template-rows: auto;
  grid-template-areas: 'logo links';
  vertical-align: middle;
}

#logo {
  display: inline-block;
  grid-area: logo;
}

#logo > a {
  text-decoration: none;
}

#links {
  grid-area: links;
  display: flex;
  align-items: center;
  justify-content: flex-end;
}

#links > a {
  display: block;
  color: black !important;
}

img,
#links > a:not(:last-child) {
  margin-right: 16px;
}
</style>
