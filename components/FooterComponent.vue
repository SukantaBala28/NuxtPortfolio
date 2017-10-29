<template>
	<div class="footer">
	  <div class="main-footer">
	  	<div class="container">
		    <div class="row">
	  			<div class="col-md-4 mainfooterLeft">
	  				<div class="">
	  					<h5 class="text-left marginLeft">Header Menu</h5><br/>
	  					<ul>
	  						<a v-scroll-to="'#about'"><li>About</li></a>
	  						<a v-scroll-to="'#services'"><li>Services</li></a>
	  						<a v-scroll-to="'#portfolio'"><li>Portfolio</li></a>
	  						<a v-scroll-to="'#team'"><li>Our Team</li></a>
	  						<a v-scroll-to="'#feedback'"><li>Client Feedback</li></a>
	  						<a v-scroll-to="'#contact'"><li>Contact With Me</li></a>
	  					</ul>
	  				</div>
	  			</div>
	  			<div class="col-md-4 mainfooterMiddle">
	  				<div class="">
	  					<h5 class="text-left marginLeft">Personal Link</h5><br/>
			  			<ul>
	  						<a href="#"><li>Curriculam Vitae</li></a>
	  						<a href="#"><li>Bangla Blog</li></a>
	  						<a href="#"><li>English Blog</li></a>
	  						<a href="#"><li>General Queries</li></a>
	  					</ul>
			  		</div>
	  			</div>
	  			<div class="col-md-4">
	  				<div class="text-center">
			  			<h5>Connect With Me</h5>
			  			<br/>
			  		</div>
			  		<div class="row">
			  			<div class="col-lg-6">
			  				<a href="https://github.com/SukantaBala28" title="Go to my Github profile">
				  				<div class="social-div1 github">
				  					<p class="social-link"><i class="fa fa-github-alt" aria-hidden="true"></i></p>
				  				</div>
				  			</a>
			  			</div>
			  			<div class="col-lg-6">
			  				<a href="https://www.linkedin.com/in/sukanta-bala-461418117/" title="Go to my Linkedin profile">
				  				<div class="social-div2 linkedin">
				  					<p class="social-link"><i class="fa fa-linkedin" aria-hidden="true"></i></p>
				  				</div>
				  			</a>
			  			</div>
			  		</div>
			  		<br/>
			  		<div class="row">
			  			<div class="col-lg-6">
			  				<a href="https://stackoverflow.com/users/6295132/sukanta-bala" title="Go to my Stackoverflow profile">
				  				<div class="social-div1 twitter">
				  					<p class="social-link"><i class="fa fa-stack-overflow" aria-hidden="true"></i></p>
				  				</div>
				  			</a>
			  			</div>
			  			<div class="col-lg-6">
			  				<a href="https://www.facebook.com/sukanta.bala28" title="Go to my Facebook profile">
				  				<div class="social-div2 facebook">
				  					<p class="social-link"><i class="fa fa-facebook" aria-hidden="true"></i></p>
				  				</div>
				  			</a>
			  			</div>
			  		</div>
	  			</div>
	  		</div>
		  </div>
	  </div>
	  <div class="subfooter">
	  	<div class="container">
	  		<div class="row">
	  			<div class="col-md-12">
	  				<div class="text-center">
	  			  	<p>&copy;2017 Sukanta Bala's personal portfolio</p>
	  				</div>
	  			</div>
	  		</div>
	  	</div>
	  </div>
	</div>
</template>

<script>
export default {
}
</script>

<style scoped>
.main-footer{
	padding: 100px 0px;
	background-color: #F6F6F6;
}
.mainfooterLeft, .mainfooterMiddle{
	border-right: 2px solid #ccc;
}
.mainfooterLeft ul li, .mainfooterMiddle ul li{
	list-style-type:none;
	text-align:left;
	margin-left:60px;
}
.mainfooterLeft ul a{
	cursor:pointer;
}
.mainfooterLeft ul a:hover{
	text-decoration:underline;
}
.mainfooterMiddle ul a{
	color:#2C3E50!important;
}
.marginLeft{
	margin-left:100px;
}
.social-div1{
	width:60px;
	height:60px;
	float:right;
	border-radius:50%;
}
.social-div2{
	width:60px;
	height:60px;
	float:left;
	border-radius:50%;
}
.social-link{
	font-size:45px;
	color:#fff;
	padding-left: 10px;
	margin-top: -8px;
}
.subfooter{
	padding: 15px 0px 0px 0px;
	background-color: #727F80;
	color:#fff;
}
.github{
	background-color:#222222;
}
.github:hover{
	cursor:pointer;
}
.social-link:hover{
	color:#eee!important;
}
.linkedin{
	background-color:#0077B5;
}
.linkedin:hover{
	cursor:pointer;
}
.twitter{
	background-color:#00ABF0;
}
.twitter:hover{
	cursor:pointer;
	background-color:#00ABD0;
}
.facebook{
	background-color:#295295;
}
.facebook:hover{
	cursor:pointer;
	background-color:#295270;
}

@media screen and (max-width: 991px) {
	.social-div1{
		float:none;
		margin: 0 auto;
	}
	.social-div2{
		float:none;
		margin: 0 auto;
		margin-top: 20px;
	}
}

@media screen and (max-width: 767px) {
	.mainfooterLeft, .mainfooterMiddle {
		border-right:0px!important;
	}
}
</style>
