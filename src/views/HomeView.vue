<template>
        <div class="card-body" v-for="brand in Brands" :key="brand">
          <h4 class="card-title">{{ brand.brand_name }}</h4>
          <h6 class="card-title">{{brand.color}}</h6>
          <h6 class="card-title">{{brand.size}}</h6>
      </div>
 
      <div id="display">
      </div>
 

</template>
<script>
// async function getData() {
//   let data = await fetch("https://taflnne15.github.io/JSonServer/brands.json")
//   let chocolateData = await data.json()
//   let extractedData = chocolateData.Shoe_Brands
//   let display = document.querySelector("#display")
//   extractedData.forEach(chocolate => {
//       display.innerHTML +=`
//       <div class="card-body">
//           <h4 class="card-title">${chocolate.brand_name}</h4>
//           <h6 class="card-title">${chocolate.color}</h6>
//           <h6 class="card-title">${chocolate.size}</h6>
//       </div>
     
//       `
//   })
// }
// getData()
export default{
  data(){
    return{
      Brands: [
    {
        "id" : 1,
        brand_name : "Vans",
        color : "Black",
        size: "7"
    },
    {
        "id" : 2,
        brand_name : "Nike",
        color : "green and white",
        size: "6"
    },
    {
        "id" : 3,
        brand_name : "Converse",
        color : "red",
        size: "5"
    },
    {
        "id" : 4,
        brand_name : "Adidas",
        color : "balck and white",
        size: "4"
    }
    ] 
  }
    }
  }
</script>



<style lang="scss" scoped>
</style>