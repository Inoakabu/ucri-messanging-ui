<template>
  <v-layout class="rounded rounded-md">
    <v-app-bar class="nav-bar"></v-app-bar>
    <v-main class="d-flex align-center justify-center" style="min-height: 300px">
      <v-container>
        <v-row>
          <v-col v-for="(card, i) in cards" :key="i" cols="12" sm="4" md="4">
            <v-card class="mx-auto" color="primary">
              <v-card-item>
                <div>
                  <div class="text-overline mb-1">
                    <!-- {{ variant }} -->
                  </div>
                  <div class="text-h6 mb-1">{{ card.first_name }}</div>
                  <div class="text-caption">{{ card.email }}</div>
                </div>
              </v-card-item>
              <v-card-actions>
                <v-btn> Button </v-btn>
              </v-card-actions>
            </v-card>
          </v-col>
        </v-row>
      </v-container>
    </v-main>
  </v-layout>
</template>

<script setup lang="ts">
defineProps<{
  // msg: string
}>()
import { ref } from 'vue'

const cards = [
  {
    id: 1,
    first_name: 'Vance',
    last_name: 'Deeming',
    email: 'vdeeming0@jimdo.com',
    gender: 'Male',
    ip_address: '118.75.22.144'
  },
  {
    id: 2,
    first_name: 'Winny',
    last_name: 'Laughlan',
    email: 'wlaughlan1@hatena.ne.jp',
    gender: 'Female',
    ip_address: '4.232.91.59'
  },
  {
    id: 3,
    first_name: 'Dusty',
    last_name: 'Maundrell',
    email: 'dmaundrell2@printfriendly.com',
    gender: 'Female',
    ip_address: '223.252.60.176'
  },
  {
    id: 4,
    first_name: 'Rebeka',
    last_name: 'Milam',
    email: 'rmilam3@rediff.com',
    gender: 'Female',
    ip_address: '69.173.105.236'
  },
  {
    id: 5,
    first_name: 'Griffy',
    last_name: 'Dunsford',
    email: 'gdunsford4@nba.com',
    gender: 'Male',
    ip_address: '25.49.220.172'
  },
  {
    id: 6,
    first_name: 'Keary',
    last_name: 'Skoughman',
    email: 'kskoughman5@examiner.com',
    gender: 'Male',
    ip_address: '89.196.117.43'
  },
  {
    id: 7,
    first_name: 'Nikoletta',
    last_name: 'Moodycliffe',
    email: 'nmoodycliffe6@theguardian.com',
    gender: 'Female',
    ip_address: '26.162.34.160'
  },
  {
    id: 8,
    first_name: 'Kelley',
    last_name: 'Buttrick',
    email: 'kbuttrick7@epa.gov',
    gender: 'Female',
    ip_address: '9.85.180.10'
  },
  {
    id: 9,
    first_name: 'Abeu',
    last_name: 'Geely',
    email: 'ageely8@ow.ly',
    gender: 'Male',
    ip_address: '64.56.99.38'
  },
  {
    id: 10,
    first_name: 'Tory',
    last_name: 'Suermeiers',
    email: 'tsuermeiers9@ning.com',
    gender: 'Female',
    ip_address: '32.188.83.37'
  }
]
</script>

<style scoped>
.wrapper {
  left: 0px;
  top: 0px;
  position: absolute;
}

.nav-bar {
  left: 0px;
  top: 0px;
  position: absolute;
  background: #6b6b6b;
}

.main {
  background: #2c2c2c;
}
</style>
