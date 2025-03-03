# Important-  
<!DOCTYPE html>
<html>
<head>
	<title>Pedido de Fotinha</title>
	<style>
		body {
			font-family: Arial, sans-serif;
			background-color: #f0f0f0;
		}
		
		.container {
			width: 80%;
			margin: 40px auto;
			background-color: #fff;
			padding: 20px;
			border: 1px solid #ddd;
			box-shadow: 0 0 10px rgba(0, 0, 0, 0.1);
		}
		
		.botao {
			background-color: #4CAF50;
			color: #fff;
			padding: 10px 20px;
			border: none;
			border-radius: 5px;
			cursor: pointer;
		}
		
		.botao:hover {
			background-color: #3e8e41;
		}
		
		.erro {
			color: #ff0000;
			font-weight: bold;
			margin-bottom: 10px;
		}
	</style>
</head>
<body>
	<div class="container">
		<h1> me ajude a ficar feliz? </h1>
		<p>FOTINHA DO PEITINHO HOJE?</p>
		
		<button class="botao" id="sim" onclick="responderSim()">Sim</button>
		<button class="botao" id="nao" onmouseover="moverBotao()">Não</button>
		
		<div id="resultado"></div>
	</div>
	
	<script>
		function responderSim() {
			document.getElementById('resultado').innerHTML = '<span style="font-size: 24px;">😊</span> Seu amorzinho vai ficar muito feliz!';
		}
		
		function moverBotao() {
			var botaoNao = document.getElementById('nao');
			botaoNao.style.position = 'absolute';
			botaoNao.style.top = Math.random() * 200 + 'px';
			botaoNao.style.left = Math.random() * 200 + 'px';
		}
	</script>
</body>
</html>
