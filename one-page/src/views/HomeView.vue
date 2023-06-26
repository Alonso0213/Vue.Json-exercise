<template>
  <div>
<ul>
  <li class="display"> 
    
  </li>
</ul>
  </div>

  <footer />
</template>

<script>
async function retriveData() {
  let data =await fetch("https://alonso0213.github.io/json-server2/index.json")
  let people = await data.json()

  let info2 = people.class

  let display = document.querySelector(".display")

  info2.forEach(data =>{
    display.innerHTML +=`
    <li><h1>${data.name}</h1></li>
    <li><h1>${data.age}<h1></li>
    `
  })
}
retriveData()
</script>

<style  scoped>

</style>