<template>
  <div id="App">
    <HeaderSection />
    <MainSection />
    <BlueMainSection />
    <FooterSection />
    <SocialSection />
  </div>
</template>
<script>
import HeaderSection from './components/HeaderSection.vue';
import MainSection from './components/MainSection.vue';
import BlueMainSection from './components/BlueMainSection.vue';
import FooterSection from './components/FooterSection.vue';
import SocialSection from './components/SocialSection.vue';

export default {
  name: 'App',
  components: {
    HeaderSection,
    MainSection,
    BlueMainSection,
    FooterSection,
    SocialSection
}
}
</script>

<style lang="scss">

@import "./style/common.scss";

</style>
