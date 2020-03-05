# calculator
progate project
<!DOCTYPE html>
<html>
<head>
	<title>Calculator</title>


<script> 
        
         function dis(val) 
         { 
             document.getElementById("result").value+=val 
         } 
           
        
         function solve() 
         { 
             let x = document.getElementById("result").value 
             let y = eval(x) 
             document.getElementById("result").value = y 
         } 
           
      
         function clr() 
         { 
             document.getElementById("result").value = "" 
         } 
      </script>




	<style type="text/css">
		.calculator{
			text-align: center;
			margin: 0 auto;
			padding-top: 100px;
			width: 400px;
		}
		.calculator-screen{
			width: 100%;
			height: 100px;
			background-color: #252525;
			color: #fff;
			text-align: right;
			font-size: 36px;
			border:none;
			padding: 0 20px;
			box-sizing: border-box;
		}

		.calculator-keys{
			width: 100%;
		}
		.row{
			display: flex;
		}

		button{
			height: 80px;
			background-color: gray;
			border: 1px solid #000;
			font-size: 32px;
			color: #fff;
			width: 25%;
			outline: none;
		}

		.all-clear, .zero-btn{
			width: 50%;
		}

		.operator, .equal-sign{
			background-color: orange;
		}
		button:hover{
			background-color: darkgrey;
		}
		.operator:hover{
			background-color: darkorange;
		}
	</style>

</head>


<body>
	<div class="calculator">
		<input type="text" class="calculator-screen" value="0" id="result" disabled>
	<div class="calculator-keys">
	<div class="row">
		<button class="all-clear" onclick="clr()">AC</button>
		<button class="percentage">%</button>
		<button class="operator" value="/" onclick="dis('/')">&divide;</button>	
		</div>


		<div class="row">
		<button class="number" value="7" onclick="dis('7')">7</button>
		<button class="number" value="8" onclick="dis('8')">8</button>
		<button class="number" value="9" onclick="dis('9')">9</button>	
		<button class="operator" value="" onclick="dis('')">&times;</button>
		</div>


		<div class="row">
		<button class="number" value="4" onclick="dis('4')">4</button>
		<button class="number" value="5" onclick="dis('5')">5</button>
		<button class="number" value="6" onclick="dis('6')">6</button>	
		<button class="operator" value="-" onclick="dis('-')">-</button>
		</div>


        <div class="row">
		<button class="number" value="1" onclick="dis('1')">1</button>
		<button class="number" value="2" onclick="dis('2')">2</button>
		<button class="number" value="3" onclick="dis('3')">3</button>	
		<button class="operator" value="+" onclick="dis('+')">+</button>
		</div>


		<div class="row">
		<button class="number zero-btn" value="0" onclick="dis('0')">0</button>
		<button class="decimal" value=">" onclick="dis('.')">.</button>	
		<button class="equal-sign" onclick="solve()">=</button>
		</div>

	</div>
    </div>
    </div>
</body>
</html>
