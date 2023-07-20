<script>

import seatsIcon from '../assets/seatsIcon.png'

</script>

<template>
  <div class="carGrid">
    <div>
      
      <p>2020</p>


      <div class="carInfo">

      <p class="carType">Van</p>
      
      <div class="carSeats">
        <img src="../assets/seatsIcon.png" class="seatsIcon" />
        <p>6 seats</p>
      </div>

      </div>


    </div>

  </div>
</template>

<style>

.carGrid {
  display: flex;
  border-radius: 8px;
  border: 1px solid #E3E0E0;
  background: #FFF; 
  box-shadow: 0px 2px 0px 0px #F1EDED; 
  padding: 6px 10px; 
}

.carInfo {
  display: flex;
  gap: 20px;
}

.carType {
  border-radius: 8px;
  border: 1px solid #E3E0E0;
  background: #FFF; 
  box-shadow: 0px 2px 0px 0px #F1EDED; 
  padding: 6px 10px; 
}

.carSeats {
  display: flex;
  width: 110px;
  border-radius: 8px;
  border: 1px solid #E3E0E0;
  background: #FFF; 
  box-shadow: 0px 2px 0px 0px #F1EDED; 
  padding: 6px 10px; 
}


.clock {
  background-color: #28C4A0;
  border-radius: 16px; 
  padding: 4px;
  width: 30px;
  height: 30px;
}

.locationPin {
  background-color: #F8A82F;
  border-radius: 16px; 
  padding: 4px;
  width: 30px;
  height: 30px;
}

.house {
  background-color: #02ACEB;
  border-radius: 16px; 
  padding: 4px;
  width: 30px;
  height: 30px;
}

.phone {

}

</style>
