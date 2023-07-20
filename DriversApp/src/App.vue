

<script>
import DriverTile from './components/DriverTile.vue'
import FilterPanel from './components/FilterPanel.vue'
import SignInWidget from './components/SignInWidget.vue'
import DropdownMenu from './components/DropdownMenu.vue'
import CarInfo from './components/CarInfo.vue'

//assets
import logo from './assets/topleft.png'
import searchButton from './assets/magnifyingGlass.png'
import clock from './assets/clock.png'
import locationPin from './assets/locationPin.png'
import house from './assets/house.png'
import phone from './assets/phone.png'
import seatsIcon from './assets/seatsIcon.png'
//import { TheWelcome } from './components/TheWelcome.vue'
/*
 <div>
    <DriverTile startTime="2PM" endTime="8PM" name="Tom Martin" phone="519-111-1111" town="Elora" gender="Male" community="South" />
    <DriverTile startTime="2PM" endTime="8PM" name="Tom Martin" phone="519-111-1111" town="Elora" gender="Male" community="South" />
  </div>


<div class="fullFilterPanel">
  <div class="filterPanel">
    <p>Community:</p>
    <p>Gender:</p>
    <p>Capacity:</p>
    <p>Available From:</p>
    <p>Available To:</p>
    <button>Dropdown</button>
    <button>Dropdown</button>
    <button>Dropdown</button>
    <button>Dropdown</button>
    <button>Dropdown</button>

  </div>
  
  <button class="filterButton">S</button>
  
  </div>


*/

export default {

  data() {
    return {
      message: 'Hello World!'
    }
  },
  components: {
    DriverTile,
    FilterPanel,
    SignInWidget,
    DropdownMenu,
    CarInfo
  },
  methods: {
    async fetchData() {
      const url = 'http://127.0.0.1:8000/api/v1/drivers'
      this.message = await (await fetch(url)).json()
      console.log(this.message);
    }
  },
  created() {
    // fetch on init
    this.fetchData()
  },
  
}
</script>

<template>
<div class="test">

<div class="topButtons">
  <div class="topleftButtons">
    <img src="./assets/topleft.png" class="logo" />
    
    <p class="topLeftButtonsText">Drivers</p>
    <p class="topLeftButtonsText">About</p>
  </div>

  <div class="toprightButton">
    <button class="topButtonsText">Log In</button>
  </div>
</div>


  <div class="headerText">
    <h1 class="headerTitle">Connecting You to the Best Drivers</h1>
    <p class="headerParagraph">Say goodbye to the hassle of finding a reliable driver.
       Our app provides you access to a diverse and highly 
       qualified pool of drivers who have undergone a rigorous screening process.</p>
  </div>

  <FilterPanel />
  
  
  <div class="allInformation">
    
    <DriverTile />
    
  


  
    <div>
    <p class="allInformationText">Cindy's Available Cars</p>
    </div>

    <div class="AvailCarGrid">
    <CarInfo />
    <CarInfo />
    <CarInfo />
    <CarInfo />
    </div>
  </div>

  


  

</div>
 


  
  
</template>



<style>

.test {
  display: flex;
  flex-direction: column;
}

.logo {
  background-color: #28C4A0;
  border-radius: 40px; 
  padding: 12px; 
  width: 49.5px;
  
   
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


body {
  background-color: white;
}




.allInformation {
  display: flex;
  flex-direction: column;
  margin-left: 10%; 
  margin-top: 40px;
  border-radius: 16px;
  border: 1px solid #E3E0E0;
  background: #FFF;
  box-shadow: 0px 6px 0px 0px #F5F4F4; 
  padding: 25px 25px;
  justify-content: space-between;
  
  width: auto;

  gap: 16px;
  
  
}



.outerLining {
  border-radius: 16px;
  
  border: 1px solid #E3E0E0;
  background: #FFF;
  box-shadow: 0px 6px 0px 0px #F5F4F4; 
  padding: 25px 25px;
  justify-content: space-between;
  
  
  

}

.allInformationText {
  color: #040404;
  font-size: 18px; 
}

.AvailCarGrid {
  display: grid;
  grid-template-columns: auto auto;
	grid-template-rows: 80px 80px; 
  gap: 20px 20px;
  
  
  

}



.smallText {
  font-size: 15px;
  color: grey;

}












.headerTitle {
  font-size: 30px;
  font-weight: bold;
}

.headerParagraph {
  font-size: 20px;
}

.headerText {
  text-align: center;
  position: absolute;
  top: 20%;
  right: 20%;
  left: 20%;
  bottom: 20%;
  
}

.topButtonsText {
  font-size: 20px;
  padding: 7px 20px; 
  border-radius: 8px;
  background: #28C4A0;
  color: white;
}

.topLeftButtonsText {
  
  color: var(--tertiary-gray-500-light, #71717A);
  text-align: center;
  
  font-size: 20px;
  
  font-style: normal;
  font-weight: 600;
  line-height: 24px;
}



.topButtons {
  display: flex;
   
}

.toprightButton {
  display: flex;
  
  position: absolute;
  top: 50px;
  right: 10%;

}

.topleftButtons {
  
  display: flex;
  gap: 40px;
  position: absolute;
  top: 50px;
  left: 10%;
  font-size: 20px;
  
}



.PageTitle {
  color: white;
}

h1 {
  color: black;
}

p {
  color: black;

}
 
</style>

