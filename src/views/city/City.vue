<template>
  <div class="">
    <city-header></city-header>
    <city-search></city-search>
    <city-list></city-list>
    <city-alphabet></city-alphabet>
  </div>
</template>

<script>
import CityHeader from "../../city-components/Header";
import CitySearch from "../../city-components/Search";
import CityList from "../../city-components/List";
import CityAlphabet from "../../city-components/Alphabet";
export default {
  name: "City",
  components: {
    CityHeader,
    CitySearch,
    CityList,
    CityAlphabet
  }
};
</script>

<style></style>
