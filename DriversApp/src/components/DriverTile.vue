<script>

import clock from '../assets/clock.png'
import locationPin from '../assets/locationPin.png'
import house from '../assets/house.png'
import phone from '../assets/phone.png'


</script>

<template>
  
  <div class="driverInfo">
    <div class="driverDetails">
      <div>
      <p class="driverName">Cindy S.</p>
      <P class="driverSmallText">Female</p>
      </div>

      <div>
      <p class="driverSmallText">Available Time</p>
      <div class="driverContainer">
      <img src="../assets/clock.png" class="clock" />
      <p class="driverMediumText">8:00AM-5:00PM</p>
      </div>
      </div>


      <div>
      <p class="driverSmallText">Location</p>
      <div class="driverContainer">
      <img src="../assets/locationPin.png" class="locationPin" />
      <p class="driverMediumText">South</p>
      </div>
      </div>

      <div>
      <p class="driverSmallText">Town</p>
      <div class="driverContainer">
      <img src="../assets/house.png" class="house" />
      <p class="driverMediumText">Fergus</p>
      </div>
      </div>

      

      

      


    </div>
    <div class="driverPhone">
      <img src="../assets/phone.png" class="phone" />
      <p class="driverPhoneText">519-111-1111</p>
    </div>
  </div>

</template>

<style>

.driverContainer {
  display: flex;
  
}

.driverInfo {
  
  display: flex;
  width: auto;
  height: auto;
  
  border-radius: 16px;
  border: 1px solid #E3E0E0;
  background: #FFF;
  box-shadow: 0px 6px 0px 0px #F5F4F4; 
  padding: 25px 25px;
  justify-content: space-between;
  align-items: center; 
  

}




.driverDetails {
  display: grid;
  grid-template-columns: 150px 200px 150px 150px;
	grid-template-rows: 40px; 
	gap: 90px 90px;
}

.driverName {
  color: #040404;
  font-size: 24px; 
}

.driverSmallText {
  color: #71717A;
  font-size: 16px; 
}

.driverMediumText {
  color: #040404;
  font-size: 18px; 
}

.driverPhone {
  display: flex;
  padding: 10px 20px 10px 16px;
  flex-direction: row; 
  border-radius: 52px;
  background: #28C4A0; 
  gap: 6px;
  margin-right: 20%;
}

.driverPhoneText {
  color: #040404;
  font-size: 20px; 
  color: white;
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
