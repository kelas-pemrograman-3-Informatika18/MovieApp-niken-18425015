<template>
<div class="q-pa-md-row items-start q-gutter-md">
  <q-card class="my-card" flat bordered>
      <q-img
        src="~src/berandatentang.jpg"
      />

      <q-card-section>
        <div class="text-overline text-orange-9">Overline</div>
        <div class="text-h5 q-mt-sm q-mb-xs">Title</div>
        <div class="text-caption text-grey">
          kalian bisa membeli DVD kesukaan kalian lewat website ini,
          dengan metode pembayaran transfer melalui bank apa saja.
          semoga kalian puas untuk berbelanja dvd di website ini.
        </div>
      </q-card-section>

      <q-card-actions>
        <q-btn flat color="dark" label="Share" />
        <q-btn flat color="primary" label="Book" />

        <q-space />

        <q-btn
          color="cyan-2"
          round
          flat
          dense
          :icon="expanded ? 'keyboard_arrow_up' : 'keyboard_arrow_down'"
          @click="expanded = !expanded"
        />
      </q-card-actions>

      <q-slide-transition>
        <div v-show="expanded">
          <q-separator />
          <q-card-section class="text-subitle2">
            {{ lorem }}
          </q-card-section>
        </div>
      </q-slide-transition>
    </q-card>
  </div>

</template>
