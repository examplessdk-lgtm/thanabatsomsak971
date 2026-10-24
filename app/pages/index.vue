<script setup lang="ts">
const email = ref('')
const city = ref('')

const cities = ['กรุงเทพมหานคร', 'เชียงใหม่', 'ภูเก็ต']
</script>

<template>
  <div class="min-h-screen bg-default text-default">
    <header class="flex items-center justify-between border-b border-default px-4 py-3">
      <span class="font-mono text-sm text-highlighted">nuxt-ui-starter</span>
      <ColorModeToggle />
    </header>

    <main class="mx-auto max-w-2xl space-y-8 p-8">
      <section class="space-y-2">
        <h1 class="text-2xl font-bold text-highlighted">ธีมพร้อมใช้งาน</h1>
        <p class="text-muted">
          คอมโพเนนต์ทั้งหมดด้านล่างใช้ชุดสี custom-primary และ custom-neutral โดยอัตโนมัติ
        </p>
      </section>

      <section class="flex flex-wrap gap-3">
        <UButton label="Primary" />
        <UButton label="Secondary" color="secondary" variant="outline" />
        <UButton label="Neutral Ghost" color="neutral" variant="ghost" />
      </section>

      <section class="space-y-4">
        <UInput v-model="email" type="email" placeholder="อีเมล" class="w-full" />
        <USelect v-model="city" :items="cities" placeholder="เลือกจังหวัด" class="w-full" />
        <UTextarea :rows="3" placeholder="ข้อความ" class="w-full" />
      </section>

      <section class="grid gap-3 sm:grid-cols-3">
        <div class="rounded-md bg-muted p-4 text-muted">bg-muted</div>
        <div class="rounded-md bg-elevated p-4 text-muted">bg-elevated</div>
        <div class="rounded-md bg-accented p-4 text-muted">bg-accented</div>
      </section>
    </main>
  </div>
</template>
