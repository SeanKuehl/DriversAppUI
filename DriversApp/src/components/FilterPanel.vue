<script>


import searchButton from '../assets/magnifyingGlass.png'

</script>

<template>
  <div class="fullFilterPanel">
  <div class="filterPanel">
    <p class="filterPanelText">Community:</p>
    <p class="filterPanelText">Gender:</p>
    <p class="filterPanelText">Capacity:</p>
    <p class="filterPanelText">From:</p>
    <p class="filterPanelText">To:</p>
    <button class="dropdown">Dropdown</button>
    <button class="dropdown">Dropdown</button>
    <button class="dropdown">Dropdown</button>
    <button class="dropdown">Dropdown</button>
    <button class="dropdown">Dropdown</button>
    

  </div>
  
  <img src="../assets/magnifyingGlass.png" class="searchButton" />
  
  </div>

  
</template>

<style>




.filterButton {
  height: auto;
  width: auto;
  padding: 20px; 
  color: white;
  font-size: 50px;
  border-radius: 14px;
  background: #28C4A0;
  
}

.fullFilterPanel {
  display: flex;
  width: 75%;
  
  padding: 14px 20px; 
  height: 16%;
  margin-top: 25%;
  margin-left: 15%;
  border: 2px solid gainsboro;
  border-radius: 10px;
  gap: 26px;
}

.filterPanel {
  display: grid;
  grid-template-columns: 125px 125px 125px 125px 125px;
	grid-template-rows: auto 40px auto; 
	gap: 20px 20px;
}

.filterPanelText {
  color: #71717A;
  font-size: 16px; 
  font-weight: 500; 
}

.dropdown {
  border-radius: 12px;
  border: 1px solid #E3E0E0;
  background: #FFF;
  width: 80%;
  box-shadow: 0px 4px 0px 0px #F5F4F4; 
}

.searchButton {
  background-color: #28C4A0;
  border-radius: 14px; 
  padding: 20px; 
  width: auto;
  height: auto;
  
}

</style>
