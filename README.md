<div align="center">
  <div class="loader"></div>
</div>

.loader {
  border: 8px solid #f3f3f3; /* Cor do fundo */
  border-top: 8px solid #3498db; /* Cor da parte superior */
  border-radius: 50%; /* Forma circular */
  width: 50px; /* Largura do loader */
  height: 50px; /* Altura do loader */
  animation: spin 1s linear infinite; /* Animação de rotação */
}

@keyframes spin {
  0% { transform: rotate(0deg); }
  100% { transform: rotate(360deg); }
}
