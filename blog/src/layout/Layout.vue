<template>
  <div>
    <Background
      style="position: fixed; z-index: -1; width: 100%; height: 100%"
      pic="2.jpg"
    />
    <!-- <Topvideo /> -->
    <Header position="fixed" title="wangblog"/>
  </div>
  <About name="首 页"/>
  <div style="display: flex;width:70%;margin:0 auto">
    <div style="width:70%">
    <router-view />
    </div>
    <div style="width:30%">
    <div style="margin:0 auto"><SelfBlock /><WarnBlock /><InfoBlock /><TagBlock /><TimeBlock /></div>
    </div>
  </div>
  <Footer />
</template>

<script>
import Topvideo from "@/components/Topvideo";
import Header from "@/components/Header";
import Footer from "@/components/Footer";
import About from "@/components/About";
import SelfBlock from "@/components/SelfBlock";
import InfoBlock from "@/components/InfoBlock";
import WarnBlock from "@/components/WarnBlock";
import TimeBlock from "@/components/TimeBlock";
import TagBlock from "@/components/TagBlock";
import Background from "../components/Background.vue";

export default {
  name: "Layout",
  components: {
    Topvideo,
    Header,
    Footer,
    About,
    SelfBlock,
    InfoBlock,
    WarnBlock,
    TimeBlock,
    TagBlock,
    Background,
  },
  data() {
    return {};
  },
};
</script>

<style scoped>
</style>