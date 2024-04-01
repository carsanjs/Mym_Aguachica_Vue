<template>

<div class="cel">
    <div class="selected-pizza">
      <img id="pizza-img" src="https://i2.wp.com/multarte.com.br/wp-content/uploads/2019/03/pizza-png-fundo-transparente20.png?fit=934%2C909&ssl=1" class="pizza-img">
    </div>

    <div class="subtitles">Choose your flavour</div>
    <div id="container" class="pizza-f-container">
      <i id="arrow-left" data-feather="chevron-left"></i>
      <i id="arrow-right" data-feather="chevron-right"></i>
      <div id="pizza-flavours" class="pizza-flavours"> </div>
    </div>

    <div class="subtitles">Size</div>
    <div id="pizza-size" class="pizza-size">
      <input type="radio" name="size" id="p" value="p" />
      <label for="p">P</label>
      <input type="radio" name="size" id="m" value="m" checked />
      <label for="m">M</label>
      <input type="radio" name="size" id="g" value="g" />
      <label for="g">G</label>
    </div>
  <div class="total-container">
    <div class="quantity">
        <i id="minus" data-feather="minus-circle"></i>
        <input type="text" class="pizza-counter" value="1" id="pizza-counter"/>
        <i id="plus" data-feather="plus-circle"></i>
    </div>
    <div class="total">$
      <span id="price">35</span>
    </div>
  </div>
    <div class="order">
      <button>Order now</button>
    </div>
</div>


</template>
<!-- <script src="https://unpkg.com/feather-icons"></script>  -->
<script setup>

    </script>

    <style>
  
@import url("https://fonts.googleapis.com/css2?family=Merriweather:wght@400;700&display=swap");

* {
  box-sizing: border-box;
}


.cel {
  background: #fff;
  width: 320px;
  height: 650px;
  border-radius: 34px;
}

.selected-pizza {
  background: center / contain no-repeat   url("https://i.imgur.com/3WPtwSm.png");
  width: 100%;
  height: 350px;
  padding: 30px 15px;

  display: flex;
  justify-content: center;
  align-items: center;
}

.pizza-img {
  width: 270px;
  transition: 0.25s ease-out;
}

input[type="radio"] {
  display: none;
}

label {
  width: 100%;
  text-align: center;
}

.subtitles {
  width: 100%;
  color: grey;
  font-size: 0.7rem;
  text-align: center;
}

#container {
  width: 100%;
  overflow: hidden;
  position: relative;
  margin-bottom: 15px;
}

.pizza-flavours {
  display: flex;
  flex-direction: row;
  justify-content: center;
  align-items: center;
  width: 300%;
  height: 50px;
  transition: 0.25s ease-in-out;
  overflow-x: scroll;
  font-weight: bold;
}

.pizza-flavours label {
  font-size: 1.4rem;
}

#arrow-left {
  height: 50px;
  top: 0;
  left: 25px;
  position: absolute;
  z-index: 99;
  color: #99101c;
}

#arrow-right {
  height: 50px;
  position: absolute;
  top: 0;
  right: 25px;
  z-index: 99;
  color: #99101c;
}

.pizza-size {
  margin: 15px 0;
  width: 100%;
  display: flex;
  justify-content: center;
}

.pizza-size {
  display: flex;
  list-style: none;
  padding: 0;
}

.pizza-size {
  input[type="radio"] {
    &:checked {
      & + label {
        color: #fff;
        border: 2px solid #99101c;
        background: #99101c;
      }
    }
  }
}

.pizza-size label {
  color: #99101c;
  width: 30px;
  height: 30px;
  border: 2px solid #99101c;
  border-radius: 50%;
  margin: 0 15px;
  display: flex;
  justify-content: center;
  align-items: center;
}

button {
  font-family: "Merriweather", serif;
  font-size: 1rem;
  font-weight: bold;
  background: #99101c;
  border: 2px solid #99101c;
  color: #fff;
  border-radius: 16px;
  padding: 7px 20px;
}

.order {
  width: 100%;
  display: flex;
  justify-content: center;
}

.pizza-counter {
  width: 40px;
  height: 40px;
  border: 0;
  font-size: 1.5rem;
  text-align: center;
  font-family: "Merriweather", serif;
  pointer-events: none;
}

.total-container {
  height: 50px;
  margin: 20px 0;
  padding: 0 15px;
  display: flex;
  align-items: center;
  justify-content: space-around;
}

.total {
  font-size: 1.5rem;
  color: #99101c;
}

</style>