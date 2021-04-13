<script>

</script>
<svelte:head>
	<title>Heath Panel</title>
	<link rel="stylesheet" href="https://cdnjs.cloudflare.com/ajax/libs/font-awesome/5.15.3/css/all.min.css" integrity="sha512-iBBXm8fW90+nuLcSKlbmrPcLa0OT92xO1BIsZ+ywDWZCvqsWgccV3gFoRBv0z+8dLJgyAHIhR35VZc2oM/gI1w==" crossorigin="anonymous" />
</svelte:head>

<div class="container">
	<div class="bg1">
	  <h2>16 <span>| 24</span></h2>
	  <p>Goals Completed</p>
	</div>
	<div class="bg1">
	  <h2><i class="fas fa-battery-three-quarters"></i></h2>
	  <p>Respiration</p>
	</div>
	<div class="bg2">
	  <h2><i class="fas fa-running"></i></h2>
	  <p>Miles</p>
	</div>
	<div class="bg1">
	  <h2>36 &deg;</h2>
	  <p>Temperature</p>
	</div>
	<div class="bg1">
	  <h2><i class="fas fa-bed"></i></h2>
	  <p>Sleep Keep</p>
	</div>
	<div class="bg2">
	  <h2>98 <span>bpm</span></h2>
	  <p>Heart Rate</p>
	</div>
	<div class="bg1">
	  <h2>170 <span>lbs</span></h2>
	  <p>Weight</p>
	</div>
	<div class="bg1">
	  <h2>28 <span>%</span></h2>
	  <p>Fat Percentage</p>
	</div>
	<div class="bg2">
	  <h2>118 <span>mgdl</span></h2>
	  <p>Blood Glucose</p>
	</div>
	<div class="bg2">
	  <h2>680 <span>kcal</span></h2>
	  <p>AVG Consumption</p>
	</div>
	<div class="bg2">
	  <h2><i class="fas fa-dumbbell"></i></h2>
	  <p>Workouts</p>
	</div>
	<div class="bg2">
	  <h2>85 <span>%</span></h2>
	  <p>Body Hydration</p>
	</div>
  </div>

  <style>

	@import url('https://fonts.googleapis.com/css2?family=Roboto:wght@300;400&display=swap');
	*{
		box-sizing: border-box;
		margin: 0;
		padding: 0;
	}
	:global(body){
		background: #333;
		color: #fff;
		font-family: 'Roboto', sans-serif;
	}

	h2{
		font-size: 45px;
		font-weight: 300;
		margin: 10px;
	}
	h2 span{
		font-size: 30px;
	}
	p{
		font-size: 20px;
	}
	.container{
		display: grid;
		grid-template-columns: repeat(4, 1fr);
		grid-gap: 10px;
	}
	.container > div{
		cursor: pointer;
		height: 210px;		
		background-size: cover;
		background-attachment: fixed;

		display: flex;
		flex-direction: column;
		align-items: center;
		justify-content: center;
		text-align: center;

		transition: all 0.5s ease-in;
	}
	@media screen and (max-width: 600px){
		.container, div{
			display: flex;
			flex-direction: column;
		}
	}
	.container > div:hover{
		opacity: 0.7;
		transform: scale(0.98);
	}
	.container > div:nth-of-type(1){
		grid-column: 1/3;
	}
	.container > div:nth-of-type(6){
		grid-column: 3/5;
	}
	.container > div:nth-of-type(9){
		grid-column: 3/5;
	}
	.container > div:nth-of-type(10){
		grid-column: 1/3;
	}
	.bg1{
		/* background: url('/img/bg1.jpg'); */
		background: rgb(134, 3, 134);
	}
	.bg2{
		/* background: url('/img/bg2.jpg'); */
		background: rgb(228, 162, 39);
		color: #333;
	}


  </style>