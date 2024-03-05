<template>
  <nav>
    <v-app-bar color="1E1E1E" dark>
      <v-toolbar-title>
        <v-img 
        max-height="80" 
        max-width="300" 
        class="ml-4" :src="require('~/assets/mju_logo_FOOTER.png')">
        </v-img>
      </v-toolbar-title>
      <v-spacer></v-spacer>
      <v-btn text color="success" class="mr-5" @click="homepage">หน้าหลัก</v-btn>
      <v-btn text color="success" class="mr-5" @click="news">ข่าวประชาสัมพันธ์</v-btn>
      <v-btn text color="success" class="mr-5" @click="services">ระบบสารสนเทศ</v-btn>
      <v-btn text color="success" class="mr-5" @click="about">เกี่ยวกับเรา</v-btn>
      <v-btn text color="success" class="mr-5" @click="Register">สมัคร</v-btn>
      <v-btn depressed color="success" @click="login">เข้าสู่ระบบ | Log in</v-btn>

    </v-app-bar>
  </nav>
</template>

<script>
import Register from '../pages/register.vue';

export default {
  name: "navbar",
  data() {
    return {};
  },
  methods: {
    homepage() {
      this.$router.push("/");
    },
    news() {
      this.$router.push("/news");
    },
    services() {
      this.$router.push("/services");
    },
    about() {
      this.$router.push("/about");
    },
    Register() {
      this.$router.push("/register");
    },
    login() {
      this.$router.push("/login");
    },
  },
};
</script>

