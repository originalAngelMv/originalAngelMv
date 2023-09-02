### Hi there 👋
<!-- Encabezado -->
# ¡Hola! Soy Angel 👋

<!-- Contenedor del texto animado -->
<div id="animated-text"></div>

<!-- Estilo para animar el texto -->
<style>
  #animated-text {
    font-size: 24px;
    font-weight: bold;
    overflow: hidden;
    white-space: nowrap;
    border-right: 3px solid #0074d9;
    animation: typing 2s steps(40, end),
               blink-caret 0.75s step-end infinite;
  }

  @keyframes typing {
    from {
      width: 0;
    }
    to {
      width: 100%;
    }
  }

  @keyframes blink-caret {
    from,
    to {
      border-color: transparent;
    }
    50% {
      border-color: #0074d9;
    }
  }
</style>

<!-- Script para escribir el texto de manera animada -->
<script>
  const text = "Hola, soy Angel. Bienvenido a mi perfil en GitHub.";
  let index = 0;

  function type() {
    if (index < text.length) {
      document.getElementById("animated-text").innerHTML += text.charAt(index);
      index++;
      setTimeout(type, 50); // Controla la velocidad de escritura
    }
  }

  // Iniciar la animación cuando se carga la página
  window.onload = function () {
    type();
  };
</script>

<!--
**originalAngelMv/originalAngelMv** is a ✨ _special_ ✨ repository because its `README.md` (this file) appears on your GitHub profile.

Here are some ideas to get you started:

- 🔭 I’m currently working on ...
- 🌱 I’m currently learning ...
- 👯 I’m looking to collaborate on ...
- 🤔 I’m looking for help with ...
- 💬 Ask me about ...
- 📫 How to reach me: ...
- 😄 Pronouns: ...
- ⚡ Fun fact: ...
-->
