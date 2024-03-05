<template>
  <v-container :key="align" >
    <v-row no-gutter :align="align">
      <v-col v-for="n in 9"  :key="n" >
        <v-card :loading="loading" class="mx-auto my-12" max-width="350" ml-1 elevation="2" >
          <template slot="progress">
            <v-progress-linear color="success" height="10" indeterminate></v-progress-linear>
          </template>
          <v-img height="150" src="https://cdn.vuetifyjs.com/images/cards/cooking.png"></v-img>
          <v-card-title>ปูฟื้นฐานเกี่ยวกับ DATA BASE</v-card-title>
          <v-card-text>
            <v-row align="center" class="mx-0">
              <v-rating :value="4.5" color="amber" dense half-increments readonly size="14"></v-rating>

              <div class="grey--text ms-4">
                4.5 (413)
              </div>
            </v-row>

            <div class="my-4 text-subtitle-1">
              เหมาะสำหรับมือใหม่
            </div>

            <div>บทเรียนนี้มีเนื้อหาเกี่ยวกับการสอนการเริ่มต้นใช้งาน data base ต่างๆ และเรียนรู้การ coding
              ในการสร้างฐานข้อมูลที่สามารถใช้งานได้จริง</div>
          </v-card-text>
          <v-divider class="mx-4"></v-divider>

          <v-card-title>เลือกเวลาในการลงทะเบียนเพื่อเรียน</v-card-title>

          <v-card-text>
            <v-chip-group v-model="selection" active-class="success accent-4 white--text" column>
              <v-chip>8:30AM</v-chip>

              <v-chip>10:00AM</v-chip>

              <v-chip>14:30PM</v-chip>
            </v-chip-group>
          </v-card-text>

          <v-card-actions>
            <v-btn color="success lighten-2" text @click="reserve2">
              ลงทะเบียน
            </v-btn>
          </v-card-actions>
        </v-card>
      </v-col>
    </v-row>
  </v-container>
</template>

<script>
export default {
  data: () => ({
    loading: false,
    selection: 1,
    alignments: [
        'start',
        'center',
        'end',
      ],
  }),

  methods: {
    reserve1() {
      this.loading = true

      setTimeout(() => (this.loading = false), 2000)
    },

    reserve2() {
      this.loading = true

      setTimeout(() => (this.loading = false), 2000)
    },

    reserve3() {
      this.loading = true

      setTimeout(() => (this.loading = false), 2000)
    },
  },
}
</script>

<style></style>
