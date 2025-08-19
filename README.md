<!DOCTYPE html>
<html lang="pt-br">
<head>
  <meta charset="UTF-8" />
  <meta name="viewport" content="width=device-width, initial-scale=1.0" />
  <title>Fox Gym - Loja de Suplementos</title>
  <script src="https://cdn.tailwindcss.com"></script>
  <link rel="stylesheet" href="https://cdn.jsdelivr.net/npm/swiper@10/swiper-bundle.min.css" />
  <style>
    @import url('https://fonts.googleapis.com/css2?family=Inter:wght@400;700&display=swap');
    body {
      font-family: 'Inter', sans-serif;
    }
    .whatsapp-btn {
      position: fixed;
      bottom: 20px;
      right: 20px;
      background: #25D366;
      color: white;
      padding: 12px 16px;
      border-radius: 50%;
      font-size: 24px;
      box-shadow: 0 4px 6px rgba(0,0,0,0.3);
      z-index: 1000;
      text-align: center;
      line-height: 1;
      display: flex;
      justify-content: center;
      align-items: center;
    }
    .pix-modal {
      position: fixed;
      top: 0; left: 0;
      width: 100%; height: 100%;
      background: rgba(0,0,0,0.7);
      display: none;
      justify-content: center;
      align-items: center;
      z-index: 1001;
    }
    .pix-content {
      background: white;
      padding: 20px;
      border-radius: 8px;
      text-align: center;
      max-width: 320px;
      width: 90%;
    }
    /* Animação de entrada */
.carrinho-item {
  transition: transform 0.3s, opacity 0.3s;
}
.carrinho-item.entrada {
  transform: translateX(20px);
  opacity: 0;
  animation: entrar 0.3s forwards;
}

@keyframes entrar {
  to {
    transform: translateX(0);
    opacity: 1;
  }
}

/* Animação de saída */
.carrinho-item.saida {
  transform: translateX(0);
  opacity: 1;
  animation: sair 0.3s forwards;
}

@keyframes sair {
  to {
    transform: translateX(20px);
    opacity: 0;
  }
}

 section img { 
  max-width: 50%;
  height: auto;
  display: block;
  
}

  </style>
</head>

<body class="bg-gray-100 text-gray-800">

  <!-- WhatsApp -->
  <a href="https://wa.me/5533984430371" target="_blank" class="whatsapp-btn" aria-label="WhatsApp">💬</a>

  <!-- Header -->
  <header class="bg-orange-600 text-white p-6 md:p-10 mb-10 rounded-b-xl">
    <div class="container mx-auto text-center">
      <h1 class="text-4xl md:text-6xl font-bold mb-2">Fox Gym</h1>
      <p class="text-lg md:text-xl">Suplementos com design exclusivo</p>
    </div>
  </header>
<div class="text-center mb-4">
  <a href="Untitled-1.html" class="text-blue-500 dark:text-blue-400 hover:underline">
    Voltar para login
  </a>
</div>
 <div class="text-center mb-4">
  <a href="Untitled-4.html" class="text-blue-500 dark:text-blue-400 hover:underline">
    Voltar para a página principal
  </a>
</div>

  <!-- Carrossel Swiper.js -->
  <section class="container mx-auto mb-10">
    <h2 class="text-3xl font-bold text-center text-orange-600 mb-6">Destaques</h2>
    <div class="swiper mySwiper">
      <div class="swiper-wrapper">
        <div class="swiper-slide"><img src="whay.png" class="w-full rounded-xl" alt="Whey Protein Fox Gym" /></div>
        <div class="swiper-slide"><img src="creatina.png" class="w-full rounded-xl" alt="Creatina Fox Gym" /></div>
        <div class="swiper-slide"><img src="pre trino.png" class="w-full rounded-xl" alt="Pré-Treino Fox Gym" /></div>
        <div class="swiper-slide"><img src="bcaa.png" class="w-full rounded-xl" alt="BCAA Fox Gym" /></div>
        <div class="swiper-slide"><img src="Gemini_Generated_Image_zcb16azcb16azcb1.png" class="w-full rounded-xl" alt="Glutamina Fox Gym" /></div>
      </div>
      <div class="swiper-pagination"></div>
    </div>
  </section>

  <!-- Loja / Carrinho -->
  <section class="container mx-auto px-4 mb-16">
    <h2 class="text-3xl font-bold text-orange-600 mb-6">Loja Fox Gym</h2>
    <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 mb-6">
      
     <body>
      <h2 class="topico-suplementos">Suplementos</h2>

<style>
  .topico-suplementos {
    text-align: center;   /* Centraliza horizontal */
    font-size: 500%;
    color: #b35f00;
    margin: 100px 0;
  }
</style>
     </body>

      <!-- Whey -->

      <div class="bg-white p-4 rounded-xl shadow">
        <img src="whay.png" alt="Whey" class="mb-2 rounded" />
        <h3 class="text-xl font-semibold">Whey Protein</h3>
        <p class="text-orange-600 font-bold">R$ 129,90</p>
        <button onclick="addToCart('Whey Protein',129.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
      </div>
      <!-- Creatina -->
      <div class="bg-white p-4 rounded-xl shadow">
        <img src="creatina.png" alt="Creatina" class="mb-2 rounded" />
        <h3 class="text-xl font-semibold">Creatina</h3>
        <p class="text-orange-600 font-bold">R$ 89,90</p>
        <button onclick="addToCart('Creatina',89.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
      </div>
      <!-- Pré-Treino -->
      <div class="bg-white p-4 rounded-xl shadow">
        <img src="pre trino.png" alt="Pré-Treino" class="mb-2 rounded" />
        <h3 class="text-xl font-semibold">Pré-Treino</h3>
        <p class="text-orange-600 font-bold">R$ 99,90</p>
        <button onclick="addToCart('Pré-Treino',99.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
      </div>
      <!-- BCAA -->
      <div class="bg-white p-4 rounded-xl shadow">
        <img src="bcaa.png" alt="BCAA" class="mb-2 rounded" />
        <h3 class="text-xl font-semibold">BCAA</h3>
        <p class="text-orange-600 font-bold">R$ 79,90</p>
        <button onclick="addToCart('BCAA',79.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
      </div>
      <!-- Glutamina -->
      <div class="bg-white p-4 rounded-xl shadow">
        <img src="Gemini_Generated_Image_zcb16azcb16azcb1.png" alt="Glutamina" class="mb-2 rounded" />
        <h3 class="text-xl font-semibold">Glutamina</h3>
        <p class="text-orange-600 font-bold">R$ 69,90</p>
        <button onclick="addToCart('Glutamina',69.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
      </div>
    </div>
    <title>Mais informações no link abaixo</title>
</head>
<body>
    <h1>Mais informações no link abaixo 👇</h1>
    
    <!-- Link simples -->
    <a href="t3.html" target="_blank">
        saiba mais
    </a>
</body>
<!-- Calculadora de Frete com Cidade pelo CEP -->
<div id="frete-container" style="max-width: 400px; margin: 50px auto; padding: 20px; background: #fff; border-radius: 10px; box-shadow: 0 4px 10px rgba(0,0,0,0.1); font-family: Arial, sans-serif;">
  <h3 style="text-align:center; color:#1d4ed8;">Calculadora de Frete</h3>
  <input type="number" id="frete-valor" placeholder="Valor do pedido (R$)" style="width:100%; padding:10px; margin:10px 0; border-radius:5px; border:1px solid #ccc;">
  <input type="text" id="frete-cep" placeholder="CEP de destino (somente números)" style="width:100%; padding:10px; margin:10px 0; border-radius:5px; border:1px solid #ccc;">
  <button id="frete-calcular" style="width:100%; padding:10px; background:#1d4ed8; color:white; border:none; border-radius:5px; cursor:pointer;">Calcular Frete</button>
  <div id="frete-resultado" style="margin-top:20px; font-size:1.1em; color:#1f2937; text-align:center;"></div>
</div>

<script>
(function(){
  const btn = document.getElementById('frete-calcular');
  btn.addEventListener('click', async function() {
    const valor = parseFloat(document.getElementById('frete-valor').value);
    const cep = document.getElementById('frete-cep').value.replace(/\D/g, '');
    const resultado = document.getElementById('frete-resultado');

    if (isNaN(valor) || valor < 0) {
      alert("Digite um valor válido do pedido.");
      return;
    }

    if (!cep || cep.length !== 8) {
      alert("Digite um CEP válido (8 números).");
      return;
    }

    let frete = 0;

    // Lógica simples de frete
    if (valor >= 200) {
      frete = 0; // frete grátis
    } else if (cep.startsWith('0') || cep.startsWith('1')) {
      frete = 12;
    } else if (cep.startsWith('2') || cep.startsWith('3')) {
      frete = 18;
    } else {
      frete = 25;
    }

    const total = valor + frete;

    try {
      // Consulta ViaCEP para obter cidade
      const response = await fetch(`https://viacep.com.br/ws/${cep}/json/`);
      const data = await response.json();
      const cidade = data.localidade || "Cidade não encontrada";

      resultado.innerHTML = `
        Valor do pedido: R$ ${valor.toFixed(2)} <br>
        Frete: R$ ${frete.toFixed(2)} <br>
        Cidade de destino: ${cidade} <br>
        <strong>Total a pagar: R$ ${total.toFixed(2)}</strong>
      `;
    } catch (error) {
      resultado.innerHTML = "Erro ao buscar a cidade pelo CEP.";
    }
  });
})();
</script>

    <div class="mt-8">
      <h3 class="text-xl font-bold mb-2">🛒 Carrinho:</h3>
      <ul id="cartItems" class="list-disc list-inside text-gray-700"></ul>
      <p class="mt-2 font-semibold">Total: R$ <span id="cartTotal">0,00</span></p>
      <button onclick="openPix()" class="mt-4 bg-green-600 text-white px-6 py-2 rounded hover:bg-green-700">Pagar com PIX</button>
    </div>
  </section>
     <section>
        <div class="grid grid-cols-1 sm:grid-cols-2 md:grid-cols-3 gap-6 mb-6">
          
  <!-- Produtos já existentes... (Whey, Creatina, etc.) -->
     <body>
      <h2 class="topico-acessorios">Acessórios</h2>

<style>
  .topico-acessorios {
    text-align: center;   /* Centraliza horizontal */
    font-size: 500%;
    color: #b35f00;
    margin: 100px 0;
  }
</style>
     </body>
  <!-- Luvas de Treino -->
  <div class="bg-white p-4 rounded-xl shadow">
    <img src="luvas.png" alt="Luvas de Treino" class="mb-2 rounded" />
    <h3 class="text-xl font-semibold">Luvas de Treino</h3>
    <p class="text-orange-600 font-bold">R$ 49,90</p>
    <button onclick="addToCart('Luvas de Treino',49.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
  </div>

  <!-- Cinto de Levantamento -->
  <div class="bg-white p-4 rounded-xl shadow">
    <img src="cinto.png" alt="Cinto de Levantamento" class="mb-2 rounded" />
    <h3 class="text-xl font-semibold">Cinto de Levantamento</h3>
    <p class="text-orange-600 font-bold">R$ 119,90</p>
    <button onclick="addToCart('Cinto de Levantamento',119.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
  </div>

  <!-- Garrafa Térmica -->
  <div class="bg-white p-4 rounded-xl shadow">
    <img src="garafa.png" alt="Garrafa Térmica" class="mb-2 rounded" />
    <h3 class="text-xl font-semibold">Garrafa Térmica 1L</h3>
    <p class="text-orange-600 font-bold">R$ 59,90</p>
    <button onclick="addToCart('Garrafa Térmica 1L',59.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
  </div>

  <!-- Faixa de Resistência -->
  <div class="bg-white p-4 rounded-xl shadow">
    <img src="faixa resistencia.png" alt="Faixa de Resistência" class="mb-2 rounded" />
    <h3 class="text-xl font-semibold">Faixa de Resistência</h3>
    <p class="text-orange-600 font-bold">R$ 34,90</p>
    <button onclick="addToCart('Faixa de Resistência',34.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
  </div>

  <!-- Mochila Esportiva -->
  <div class="bg-white p-4 rounded-xl shadow">
    <img src="mochila (2).png" alt="Mochila Esportiva" class="mb-2 rounded" />
    <h3 class="text-xl font-semibold">Mochila Esportiva</h3>
    <p class="text-orange-600 font-bold">R$ 139,90</p>
    <button onclick="addToCart('Mochila Esportiva',139.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
  </div>

  <!-- Toalha de Treino -->
  <div class="bg-white p-4 rounded-xl shadow">
    <img src="toalha.png" alt="Toalha de Treino" class="mb-2 rounded" />
    <h3 class="text-xl font-semibold">Toalha de Treino</h3>
    <p class="text-orange-600 font-bold">R$ 29,90</p>
    <button onclick="addToCart('Toalha de Treino',29.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
  </div>
</div>
 <section>

     <body>
      <h2 class="topico-equipamentos">equipamentos</h2>

<style>
  .topico-equipamentos {
    text-align: center;   /* Centraliza horizontal */
    font-size: 500%;
    color: #b35f00;
    margin: 100px 0;
  }
</style>
     </body>
    <!-- Halteres Ajustáveis -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="alteres (2).webp" alt="Halteres Ajustáveis" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Halteres Ajustáveis (até 24kg)</h3>
  <p class="text-orange-600 font-bold">R$ 699,90</p>
  <button onclick="addToCart('Halteres Ajustáveis (até 24kg)',699.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

<!-- Barra W -->
<div class="bg-white p-2 rounded-xl shadow">
  <img src="images.png" alt="Barra W" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Barra W (Rosca Direta)</h3>
  <p class="text-orange-300 font-bold">R$ 229,90</p>
  <button onclick="addToCart('Barra W (Rosca Direta)',229.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

<!-- Anilha Olímpica 10kg -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="anilha.webp" alt="Anilha Olímpica 10kg" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Anilha Olímpica 10kg</h3>
  <p class="text-orange-600 font-bold">R$ 129,90</p>
  <button onclick="addToCart('Anilha Olímpica 10kg',129.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

<!-- Suporte para Halteres -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="alteres.webp" alt="Suporte para Halteres" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Suporte para Halteres</h3>
  <p class="text-orange-600 font-bold">R$ 499,90</p>
  <button onclick="addToCart('Suporte para Halteres',499.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

<!-- Banco Regulável -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="banco.webp" alt="Banco Regulável" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Banco Regulável para Musculação</h3>
  <p class="text-orange-600 font-bold">R$ 599,90</p>
  <button onclick="addToCart('Banco Regulável para Musculação',599.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

<!-- Cadeira Extensora -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="cadeira.webp" alt="Cadeira Extensora" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Cadeira Extensora</h3>
  <p class="text-orange-600 font-bold">R$ 2.499,90</p>
  <button onclick="addToCart('Cadeira Extensora',2499.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>
<section>
   

<!-- Corda Naval -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="corda.jpeg" alt="Corda Naval" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Corda Naval 12m</h3>
  <p class="text-orange-600 font-bold">R$ 399,90</p>
  <button onclick="addToCart('Corda Naval 12m',399.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

<!-- Tapete de Yoga -->
<div class="bg-white p-4 rounded-xl shadow">
  <img src="ioga.webp" alt="Tapete de Yoga" class="mb-2 rounded" />
  <h3 class="text-xl font-semibold">Tapete de Yoga Antiderrapante</h3>
  <p class="text-orange-600 font-bold">R$ 89,90</p>
  <button onclick="addToCart('Tapete de Yoga Antiderrapante',89.90)" class="mt-2 bg-orange-600 text-white px-4 py-2 rounded hover:bg-orange-700">Adicionar</button>
</div>

</section>
 </section>
     </section>
  <!-- Modal PIX -->
  <div id="pixModal" class="pix-modal" role="dialog" aria-modal="true" aria-labelledby="pixTitle" aria-hidden="true">
    <div class="pix-content">
      <h2 id="pixTitle" class="text-2xl font-bold mb-4">Pague com PIX</h2>
      <!-- Aqui vai o seu QR Code real -->
      <img src="capture_250816_084528.png" alt="PIX QR Code" class="mx-auto mb-4" />
      <button onclick="closePix()" class="bg-gray-500 text-white px-4 py-2 rounded">Fechar</button>
      <p class="mt-2 text-sm text-gray-500">
        Este é um exemplo. Em um site real, esta imagem seria um QR Code gerado dinamicamente para o pagamento.
      </p>
    </div>
  </div>

  <!-- Formulário Contato -->
  <section class="container mx-auto bg-white p-6 rounded-xl shadow-md mb-16">
    <h2 class="text-3xl font-bold text-orange-600 mb-4">Fale Conosco</h2>
    <form action="https://formspree.io/f/mayzklaw" method="POST" class="space-y-4">
      <div>
        <label class="block text-sm font-medium" for="name">Nome</label>
        <input type="text" id="name" name="name" required class="w-full border rounded px-4 py-2" />
      </div>
      <div>
        <label class="block text-sm font-medium" for="email">Email</label>
        <input type="email" id="email" name="email" required class="w-full border rounded px-4 py-2" />
      </div>
      <div>
        <label class="block text-sm font-medium" for="message">Mensagem</label>
        <textarea id="message" name="message" rows="4" required class="w-full border rounded px-4 py-2"></textarea>
      </div>
      <button type="submit" class="bg-orange-600 text-white px-6 py-2 rounded hover:bg-orange-700">Enviar</button>
    </form>
  </section>
 
  <!-- Rodapé -->
  <footer class="bg-orange-600 text-white text-center p-6 mt-10 rounded-t-xl">
    <p>&copy; 2025 Fox Gym. Todos os direitos reservados.</p>
    <p class="text-sm mt-1">Instagram: <a href="https://www.instagram.com/arlen_165" target="_blank" class="underline">foxgymoficial</a></p>
  </footer>

  <!-- Scripts -->
  <script src="https://cdn.jsdelivr.net/npm/swiper@10/swiper-bundle.min.js"></script>
  <script>
    // Swiper
    new Swiper(".mySwiper", {
      loop: true,
      pagination: { el: ".swiper-pagination", clickable: true }
    });
    

    // Carrinho com localStorage
    function getCart() {
      return JSON.parse(localStorage.getItem('cart')) || { items: [], total: 0 };
    }
    function saveCart(cart) {
      localStorage.setItem('cart', JSON.stringify(cart));
    }
    function renderCart() {
      const cart = getCart();
      const listEl = document.getElementById('cartItems');
      listEl.innerHTML = '';

      cart.items.forEach((item, index) => {
        const li = document.createElement('li');
        li.classList.add('flex', 'justify-between', 'items-center', 'mb-1');
        li.innerHTML = `
          <span>${item.name} — R$ ${item.price.toFixed(2)}</span>
          <button onclick="removeFromCart(${index})" class="text-red-600 hover:underline text-sm ml-4">Remover</button>
        `;
        listEl.appendChild(li);
      });

      document.getElementById('cartTotal').innerText = cart.total.toFixed(2).replace('.', ',');
    }
    function addToCart(name, price) {
      const cart = getCart();
      cart.items.push({ name, price });
      cart.total += price;
      saveCart(cart);
      renderCart();
    }
    function removeFromCart(index) {
      const cart = getCart();
      const item = cart.items[index];
      if (!item) return;
      cart.total -= item.price;
      cart.items.splice(index, 1);
      saveCart(cart);
      renderCart();
    }
    renderCart(); // Inicializa o carrinho

    // Funções PIX
    function openPix() {
      const modal = document.getElementById('pixModal');
      modal.style.display = 'flex';
      modal.setAttribute('aria-hidden', 'false');
    }
    function closePix() {
      const modal = document.getElementById('pixModal');
      modal.style.display = 'none';
      modal.setAttribute('aria-hidden', 'true');
    }
  </script>
  <script src="https://cdn.jsdelivr.net/npm/swiper@10/swiper-bundle.min.js"></script>
<script>
  // Swiper
  new Swiper(".mySwiper", {
    loop: true,
    pagination: { el: ".swiper-pagination", clickable: true }
  });

  // Carrinho com localStorage
  function getCart() {
    return JSON.parse(localStorage.getItem('cart')) || { items: [], total: 0 };
  }
  function saveCart(cart) {
    localStorage.setItem('cart', JSON.stringify(cart));
  }

  function renderCart() {
    const cart = getCart();
    const listEl = document.getElementById('cartItems');
    listEl.innerHTML = '';

    cart.items.forEach((item, index) => {
      const li = document.createElement('li');
      li.classList.add('flex', 'justify-between', 'items-center', 'mb-2');
      li.innerHTML = `
        <div>
          <span class="font-semibold">${item.name}</span> — 
          <span>R$ ${(item.price * item.qty).toFixed(2)}</span>
          <span class="text-sm text-gray-500">(R$ ${item.price.toFixed(2)} x ${item.qty})</span>
        </div>
        <div class="flex items-center space-x-2">
          <button onclick="updateQty(${index}, -1)" class="px-2 bg-gray-300 rounded">-</button>
          <span>${item.qty}</span>
          <button onclick="updateQty(${index}, 1)" class="px-2 bg-gray-300 rounded">+</button>
          <button onclick="removeFromCart(${index})" class="text-red-600 hover:underline text-sm">Remover</button>
        </div>
      `;
      listEl.appendChild(li);
    });

    document.getElementById('cartTotal').innerText = cart.total.toFixed(2).replace('.', ',');
  }

  function addToCart(name, price) {
    const cart = getCart();
    const existing = cart.items.find(item => item.name === name);

    if (existing) {
      existing.qty += 1;
    } else {
      cart.items.push({ name, price, qty: 1 });
    }

    cart.total += price;
    saveCart(cart);
    renderCart();
  }

  function updateQty(index, change) {
    const cart = getCart();
    const item = cart.items[index];
    if (!item) return;

    item.qty += change;

    if (item.qty <= 0) {
      cart.total -= item.price * (item.qty + 1); // remove total certo
      cart.items.splice(index, 1);
    } else {
      cart.total += item.price * change;
    }

    saveCart(cart);
    renderCart();
  }

  function removeFromCart(index) {
    const cart = getCart();
    const item = cart.items[index];
    if (!item) return;

    cart.total -= item.price * item.qty;
    cart.items.splice(index, 1);

    saveCart(cart);
    renderCart();
  }

  renderCart(); // Inicializa o carrinho

  // Funções PIX
  function openPix() {
    const modal = document.getElementById('pixModal');
    modal.style.display = 'flex';
    modal.setAttribute('aria-hidden', 'false');
  }
  function closePix() {
    const modal = document.getElementById('pixModal');
    modal.style.display = 'none';
    modal.setAttribute('aria-hidden', 'true');
  }
  // ------------------ Login/Cadastro ------------------
const loginForm = document.getElementById('loginForm');
const registerForm = document.getElementById('registerForm');
const showRegister = document.getElementById('showRegister');
const showLogin = document.getElementById('showLogin');
const authForm = document.getElementById('authForm');
const welcomeMsg = document.getElementById('welcomeMsg');
const userNameSpan = document.getElementById('userName');
const logoutBtn = document.getElementById('logoutBtn');

showRegister.addEventListener('click', e => { e.preventDefault(); loginForm.classList.add('hidden'); registerForm.classList.remove('hidden'); });
showLogin.addEventListener('click', e => { e.preventDefault(); registerForm.classList.add('hidden'); loginForm.classList.remove('hidden'); });

function getUsuarios() { return JSON.parse(localStorage.getItem('usuarios')) || []; }
function salvarUsuarios(usuarios) { localStorage.setItem('usuarios', JSON.stringify(usuarios)); }
function getUsuarioLogado() { return JSON.parse(localStorage.getItem('usuarioLogado')); }
function setUsuarioLogado(usuario) { localStorage.setItem('usuarioLogado', JSON.stringify(usuario)); }

registerForm.addEventListener('submit', e => {
  e.preventDefault();
  const nome = document.getElementById('registerName').value;
  const email = document.getElementById('registerEmail').value;
  const senha = document.getElementById('registerPassword').value;

  let usuarios = getUsuarios();
  if (usuarios.find(u => u.email === email)) { alert('Email já cadastrado!'); return; }

  usuarios.push({ nome, email, senha });
  salvarUsuarios(usuarios);
  alert('Cadastro realizado! Faça login.');
  registerForm.reset();
  registerForm.classList.add('hidden');
  loginForm.classList.remove('hidden');
});

loginForm.addEventListener('submit', e => {
  e.preventDefault();
  const email = document.getElementById('loginEmail').value;
  const senha = document.getElementById('loginPassword').value;

  const usuarios = getUsuarios();
  const usuario = usuarios.find(u => u.email === email && u.senha === senha);
  if (!usuario) { alert('Email ou senha incorretos!'); return; }

  setUsuarioLogado({ nome: usuario.nome, email: usuario.email });
  mostrarBemVindo(usuario);
  renderizarCarrinho();
});

logoutBtn.addEventListener('click', () => {
  localStorage.removeItem('usuarioLogado');
  authForm.classList.remove('hidden');
  welcomeMsg.classList.add('hidden');
});

function mostrarBemVindo(usuario) {
  authForm.classList.add('hidden');
  welcomeMsg.classList.remove('hidden');
  userNameSpan.textContent = usuario.nome;
}
</script>

</body>

</html>

