ml>
	
	<style>
		body{
			margin: 0;
		}

		.container{
			width: 100vw;
			height: 100vh;

			display: grid;
			grid-template: repeat(5, 1fr);
			grid-template-rows: 50px 1fr 1fr 50px;

			gap: 10px;
			padding: 10px;
			box-sizing: border-box;
		}

		.container div{
			padding: 10px;
			border: 1px solid rbg(255, 255, 250);
			border-radius: 10px;
		}

		.header{
			/*gridlinjenummer, linjer mellom rad og kolonne.
			Får innhold til å dra sge over flere kolonner*/
			grid-column-start: 1;
			grid-column-end: 5;
			text-align: center;
			color: red;
		}

		.box1{
			grid-row-start: 2;
			grid-row-end: 2;
			grid-column-start: 2;
			grid-column-end: 2;
			background-color: red;
		}

		.box2{
			grid-row-start: 2;
			grid-row-end: 2;
			grid-column-start: 3;
			grid-column-end: 3;
			background-color: red;
		}


		.box3{
			grid-row-start: 3;
			grid-row-end: 3;
			grid-column-start: 2;
			grid-column-end: 2;
			background-color: red;
		}

		.box4{
			grid-row-start: 3;
			grid-row-end: 3;
			grid-column-start: 3;
			grid-column-end: 3;
			background-color: red;
			border-color: blue;
		}


	</style>

	<body>
		<div class = "container">
			<div class = "header">
				<marquee scrollamount = "10" direction = "right" behaviour = "scroll">
		 			veslemøy
		 		</marquee>
			</div>
			<div class = "box1">
			</div>
			<div class = "box2">
			</div>
			<div class = "box3">
			</div>
			<div class = "box4">
			</div>
		</div>
	</body>
</html>
