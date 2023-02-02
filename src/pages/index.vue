<script setup lang="ts" generic="T extends any, O extends any">
defineOptions({
  name: 'IndexPage',
})

const thename = $ref('')

const router = useRouter()
const go = () => {
  if (thename)
    router.push(`/hi/${encodeURIComponent(thename)}`)
}
</script>

<template>
  <div>
    <SuperNavbar />
    <SuperHero />
    <div i-carbon-campsite text-4xl inline-block />
    <p>
      <a rel="noreferrer" href="https://github.com/antfu/vitesse-lite" target="_blank">
        Vitesse Lite
      </a>
    </p>
    <p>
      <em text-sm op75>Opinionated Vite Starter Template</em>
    </p>

    <div py-4 />

    <TheInput
      v-model="thename"
      placeholder="What's your name?"
      autocomplete="false"
      @keydown.enter="go"
    />

    <div>
      <button
        class="m-3 text-sm btn"
        :disabled="!thename"
        @click="go"
      >
        Go
      </button>
    </div>
  </div>
</template>
