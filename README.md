## Olá, logo logo, sai algo aqui! rs

### Carregando...

<div style="display: flex; justify-content: center; align-items: center; height: 100vh;">
  <div style="border: 16px solid #f3f3f3; border-radius: 50%; border-top: 16px solid #3498db; width: 120px; height: 120px; animation: spin 2s linear infinite;">
  </div>
  <div style="font-size: 24px; font-weight: bold; color: #333; margin-top: 20px;">Carregando...</div>
</div>

<script>
  // Simula o carregamento do conteúdo
  setTimeout(function() {
    // Remove a tela de loading
    document.querySelector("div[style*='display: flex']").style.display = "none";
    // Mostra o conteúdo
    document.querySelector("div[style*='display: none']").style.display = "block";
  }, 3000); // 3 segundos
</script>

<!-- Conteúdo que será carregado após a tela de loading -->
<div style="display: none;">
  <!-- Seu conteúdo aqui -->
</div>
