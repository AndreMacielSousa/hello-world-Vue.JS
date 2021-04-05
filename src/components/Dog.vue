<template>
  <div>
    <button @click="getDog">GET a {{ breed }}</button>
    <div>
    <img :src="dog.message" />
    </div>
  </div>
</template>

<script>
export default {
  name: "Dog",
  props: { breed: String },
  data(){
      return{
          dog: ""
      }
  },
  methods:{
      getDog: async function(){
          const response = await
          fetch(`https://dog.ceo/api/breed/${this.breed}/images/random`)
          this.dog = await response.json()
      }
  }
};
</script>
