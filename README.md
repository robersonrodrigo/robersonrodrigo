<<!DOCTYPE html>
<html>
<head>
	<title>Loading...</title>
	<style>
		.loading-container {
			display: flex;
			justify-content: center;
			align-items: center;
			height: 100vh;
			background-color: #333; /* mudança de cor de fundo */
			background-image: linear-gradient(to bottom, #333, #444); /* gradiente de fundo */
		}
		
		.loader {
			width: 150px; /* aumento do tamanho do loader */
			height: 150px;
			border-radius: 50%;
			border: 10px solid #f3f3f3;
			border-top: 10px solid #ff69b4; /* mudança de cor do loader */
			animation: spin 2s linear infinite;
			box-shadow: 0 0 20px rgba(255, 255, 255, 0.5); /* adição de sombra */
		}
		
		.loader svg {
			width: 100%;
			height: 100%;
		}
		
		.loader circle {
			stroke-dasharray: 300;
			stroke-dashoffset: 300;
			animation: dash 2s linear infinite;
		}
		
		@keyframes spin {
			0% {
				transform: rotate(0deg);
			}
			100% {
				transform: rotate(360deg);
			}
		}
		
		@keyframes dash {
			0% {
				stroke-dashoffset: 300;
			}
			50% {
				stroke-dashoffset: 0;
			}
			100% {
				stroke-dashoffset: -300;
			}
		}
		
		.loading-text {
			font-size: 36px; /* aumento do tamanho do texto */
			font-weight: bold;
			color: #fff; /* mudança de cor do texto */
			margin-top: 20px;
			text-shadow: 0 0 10px rgba(255, 255, 255, 0.5); /* adição de sombra ao texto */
		}
		
		/* adição de efeito de transição */
		.loading-container {
			transition: opacity 0.5s;
		}
		
		.loading-container:hover {
			opacity: 0.8;
		}
	</style>
</head>
<body>
	<div class="loading-container">
		<div class="loader">
			<svg viewBox="0 0 100 100">
				<circle cx="50" cy="50" r="40" fill="none" stroke-width="10" stroke="#ff69b4" />
			</svg>
		</div>
		<div class="loading-text">Carregando...</div>
	</div>
</body>
</html>
