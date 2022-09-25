<template>
  <header class="container d-flex justify-content-between">
    <div class="d-flex p-3">
      <img src="../assets/dc-logo.png" alt="dc-logo-header">
    </div>
    <ul class="d-flex justify-content-evenly align-self-center">
      <li v-for="(item, index) in headerArray" :key="index">
        {{ item.text }}
      </li>
    </ul>
  </header>
</template>

<script>
export default {

    name: 'HeaderSection',

    data: function () {
    return {
      headerArray: [
        {
          text: "CHARACTERS",
          active: false,
        },
        {
          text: "COMICS",
          active: true,
        },
        {
          text: "MOVIES",
          active: false,
        },
        {
          text: "TV",
          active: false,
        },
        {
          text: "GAMES",
          active: false,
        },
        {
          text: "COLLECTIBLES",
          active: false,
        },
        {
          text: "VIDEOS",
          active: false,
        },
        {
          text: "FANS",
          active: false,
        },
        {
          text: "NEWS",
          active: false,
        },
        {
          text: "SHOP",
          active: false,
        },
      ],
    };
  },
} 

</script>

<style lang="scss" scoped>

header {
  height: 120px;

  ul {
    list-style-type: none;
    width: 80%;
}

  li {
    border-bottom: 5px solid transparent;
    padding: 54px 0;
    font-weight: 500;

    &:hover {
      border-bottom: 5px solid #0c7cec;
    }

  }



}






</style>