<template>
  <main>
    <agile :arrows="false" :speed="1150"
    :timing="'linear'" :fade="true"
    :autoplay="true" :pauseOnHover="false">
	    <div class="slide slide--1"><h1 style="color:red">Slide 1</h1></div>
	    <div class="slide slide--2"><h1>Slide 2</h1></div>
	    <div class="slide slide--3"><h1>Slide 3</h1></div>
		</agile>
    </main>
</template>

<script>
	import Vue from 'vue'
	import VueAgile from 'vue-agile'
	Vue.use(VueAgile)

	export default {
	}
</script>

<style lang="scss" scoped>
.agile {
    &__dots {
        bottom: 0;
        display: block;
        left: 10px;
        position: absolute;
        width: 10px;
    }

    &__dot {
        margin-bottom: 10px;

        button {
            background-color: transparent;
            border: 1px solid #fff;
            margin-top: 10px;

            &:hover {
                background-color: #fff;
            }
        }

        &--current {
            button {
                background-color: #fff;
            }
        }
    }
}

.slide {
    background: {
        position: center;
        size: cover;
    }
    height: 400px;

    &--1 {
        background-image: url(../assets/img/chicago.jpg);
    }
    &--2 {
        background-image: url(../assets/img/ny.jpg);
    }
    &--3 {
        background-image: url(../assets/img/la.jpg);
    }

}
</style>
