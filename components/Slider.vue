<template>
  <div class="sliderItem">
    <div class="mySlides">
      <img src="../assets/img/la.jpg" style="width:100%">
      <div class="container">
        <h3>Los Angeles</h3>
        <p><b>We had the best time playing at Venice Beach!</b></p>   
      </div>
    </div>
    <div class="mySlides">
      <img src="../assets/img/ny.jpg" style="width:100%">
      <div class="container">
        <h3>Los Angeles</h3>
        <p><b>We had the best time playing at Venice Beach!</b></p>   
      </div>
    </div>
    <div class="mySlides">
      <img src="../assets/img/chicago.jpg" style="width:100%">
      <div class="container">
        <h3>Los Angeles</h3>
        <p><b>We had the best time playing at Venice Beach!</b></p>   
      </div>
    </div>
  </div>
</template>
<script>
	export default {
  middleware: 'authenticated'
	}
</script>

<script>
var myIndex = 0
carousel()

function carousel () {
  var i
  var x = document.getElementsByClassName('mySlides')
  for (i = 0; i < x.length; i++) {
    x[i].style.display = 'none'
  }
  myIndex++
  if (myIndex > x.length) { myIndex = 1 }
  x[myIndex - 1].style.display = 'block'
  setTimeout(carousel, 4000)
}
</script>
