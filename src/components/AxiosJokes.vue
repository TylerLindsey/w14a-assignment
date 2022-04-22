<template>
  <div>
    <div>
      <!-- it seems that i need to make 1 button that has 3 options that replace the spaces with _ on 1 of them and makes all of the letter capital on another and the 3d is just left as is.  -->
      <!-- api call needs to be made by clicking the button -->
      <!-- I need to make a GET request to https://geek-jokes.sameerkumar.website/api?format=json-->
      <!-- it needs to display in the h3 under the click button -->
      <!-- AND i need to store the joke using pinia -->
      <!-- the selection buttons need to be able to change the case, and pinia must store the joke while the components/cases changes so THAT A NEW API CALL/NEW JOKE IS NOT MADE  -->
      <h1>Axios Jokes</h1>
      <h3>Choose which case you want to see the joke in</h3>
      <SnakeCase/>
      <NormalText/>
      <p>or you could</p>
      <AllCaps/>
      <h2 id="">Click For Joke</h2> <!--In here I need to reference the API call below-->
      <h3><!--The joke from the API should display here--></h3>
    </div>
  </div>
</template>

<script>
// API call needs to be made in here somewhere
import SnakeCase from '@/components/SnakeCase.vue';
import NormalText from '@/components/NormalText.vue';
import AllCaps from '@/components/AllCaps.vue';
  export default {
    name : "AxiosJokes",
    components:{
      SnakeCase,
      NormalText,
      AllCaps
    }
  }
</script>

<style lang="scss" scoped>
h2{
  background-color: beige;
  padding: 2px;
}
</style>