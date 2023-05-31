<script>
import AppHeader from './components/AppHeader.vue';
import AppMain from './components/AppMain.vue';
import AppFooter from './components/AppFooter.vue';

export default {
  components: {AppHeader,AppMain,AppFooter},
};
</script>

<template>

<AppHeader></AppHeader>

<AppMain></AppMain>

<AppFooter></AppFooter>

</template>

<style lang="scss">
*{
  margin: auto;
  padding: auto;
  box-sizing: border-box;
}


.g-btn{
  border: none;
  background-color: #5ADDCD;
  color: white;
  padding: 8px 20px;
  margin: 15px;
  border-radius: 50px;
  text-align: center;
  cursor: pointer;
}
                  

</style>
