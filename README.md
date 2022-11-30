<html>

	<style>
		body{
			margin: 0;
		}

		/*plate der innhold legges*/
		.container{ 
			/*størrelse (vh/wh) basert på 1% person-høyde*/
			width: 100vw;
			height: 100vh;

			font-family: monaco;
			font-weight: bold;
			font-size: 10px;

			display: grid;
			/*tre kolonner med en str på 1 fraksjon av gjenværende rom*/
			grid-template-columns: repeat(5, 1fr);
			/*lar design adaptere til størrelseendring av vindu*/
			grid-template-rows: 50px 1fr 1fr 100px;

			gap: 10px;
			padding: 10px;
			box-sizing: border-box;
		}

		.container div{
			padding: 10px;
			border: 1px solid rgb(255, 228, 245);
			border-radius: 10px;
		}

		.header{
			/*gridlinjenummer, linjer mellom rad og kolonne.
			Får innhold til å dra sge over flere kolonner*/
			grid-column-start: 2;
			grid-column-end: 5;
			text-align: center;
		}

		.content{
			/* starter på 2. rad, da 1. rad er tatt av header*/
			grid-row-start: 2;
			/*drar seg over 4 rader*/
			grid-row-end: span 3;
			grid-column-start: 3;
			grid-column-end: 5;
			background-color: pink;
			overflow: auto;
			border-radius: 10px
			padding: 10px;
		}

		.sidebar{
			grid-row-start: 2;
			grid-row-end: span 3;
			grid-column-start: 2;
			grid-column-end: 2;
		}

		.footer{

			/*snarvei for de tidligere start/end-funksjonene*/
			grid-column: 2/span 3;
		}
		/*
		.box-content{
			height: 565px;
			width: 518px;
			overflow: auto;
			border-radius: 10px
			padding: 10px;
			position: relative;
		}
		*/

	</style>

	<body>
		
		 <div class = "container">
		 	<div class = "header"> 
		 		header
		 	</div>
		 	
		 	<div class = "content">
		 		content
		 	</div>
		 	<div class = "sidebar">
		 	</div>
		 	<div class = "footer">
		 		<marquee scrollamount = "10" direction = "right" behaviour = "scroll">
		 			veslemøy
		 		</marquee>
		 	</div>
		 </div>
		
	</body>
	
</html>
