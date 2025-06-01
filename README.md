# ✨ [mnrmagal.github.io](https://mnrmagal.github.io) — Seu espaço criativo online

<p align="center">
  <a href="https://mnrmagal.github.io" target="_blank">
    <img src="https://mnrmagal.github.io/favicon.ico" alt="mnrmagal logo" width="64" height="64" />
  </a>
</p>

<div align="center">

[![Open in Browser](https://img.shields.io/badge/Open-in%20Browser-brightgreen?style=for-the-badge&logo=firefox)](https://mnrmagal.github.io)
[![License](https://img.shields.io/badge/License-MIT-blue?style=for-the-badge)](https://github.com/mnrmagal/mnrmagal.github.io/blob/main/LICENSE)

</div>

---

<p align="center">
  <img src="https://i.ibb.co/4hPJnzP/grabber-by-noyato-final-60fps.gif" alt="Preview do bookmarklet mnrmagal" width="100%" />
</p>

---

## 🎯 O que é?

**[mnrmagal.github.io](https://mnrmagal.github.io)** é o seu portal para conteúdos, projetos e criações desenvolvidas por [@mnrmagal](https://github.com/mnrmagal).  
Um site moderno, direto e integrado que você pode acessar instantaneamente **sobre qualquer página da web** usando um simples **bookmarklet**.

Essa ferramenta sobrepõe o site diretamente onde você estiver navegando — sem precisar sair da aba atual. Perfeito para consultar conteúdos, ferramentas e experimentos sem interrupções.

---

## ⚡ Bookmarklet Super Prático

### 🧩 Como usar

1. Crie um **favorito** no seu navegador.
2. No campo de **URL** do favorito, cole o código abaixo:

```javascript
javascript:(function(){if(document.getElementById('mnrmagal-bookmarklet-iframe')){alert('O site já está carregado acima.');return;}var iframe=document.createElement('iframe');iframe.id='mnrmagal-bookmarklet-iframe';iframe.src='https://mnrmagal.github.io';iframe.style.position='fixed';iframe.style.top='0';iframe.style.left='0';iframe.style.width='100%';iframe.style.height='100%';iframe.style.border='none';iframe.style.zIndex='9999999';iframe.style.backgroundColor='white';var btnClose=document.createElement('button');btnClose.textContent='✕ Fechar';btnClose.id='mnrmagal-bookmarklet-close-btn';btnClose.style.position='fixed';btnClose.style.top='10px';btnClose.style.right='10px';btnClose.style.padding='10px 15px';btnClose.style.fontSize='16px';btnClose.style.zIndex='10000000';btnClose.style.cursor='pointer';btnClose.style.backgroundColor='rgba(0,0,0,0.7)';btnClose.style.color='white';btnClose.style.border='none';btnClose.style.borderRadius='5px';btnClose.style.boxShadow='0 2px 5px rgba(0,0,0,0.3)';btnClose.onclick=function(){iframe.remove();btnClose.remove();};document.body.appendChild(iframe);document.body.appendChild(btnClose);})();
