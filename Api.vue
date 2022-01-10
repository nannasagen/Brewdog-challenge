<template>
  <div>
    <h3>Brewdog beer</h3>
   
    <ul v-for="beer in beerList" v-bind:key="beer.id">
        <li>{{beer.name}}</li>
         <li>{{beer.image_url}}</li>
         <li>{{beer.abv}}</li>
        <li>{{beer.description}}</li>
        

    </ul>
  </div>
</template>

<script>
export default {
  name: "Api",
  data() {
    return {
      beerList: [],
    };
  },

  async mounted() {
    let response = await fetch("https://api.punkapi.com/v2/beers");
    let data = await response.json();
    this.beerList.push(...data);
    console.log(data);
    return data;
  },
};
</script>