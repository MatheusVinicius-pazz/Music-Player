<div align="center">
  <img src="https://res.cloudinary.com/dnrrgpoxt/image/upload/v1763465227/Gemini_Generated_Image_vx3v7rvx3v7rvx3v__1_-removebg-preview_xkkobr.png" alt="Logo VinilPlay" width="200">
  <h1>🎵 VinilPlay Experience</h1>
  
  <p>
    <strong>Sua coleção de músicas, direto da nuvem para o navegador. <a href="https://vinilplay.netlify.app/">ACESSE O SITE CLICANDO AQUI</a> •</strong> 
  </p>

  <p>
    <a href="#-sobre">Sobre</a> •
    <a href="#-funcionalidades">Funcionalidades</a> •
    <a href="#-tecnologias">Tecnologias</a> •
    <a href="#-como-rodar">Como Rodar</a> •
    <a href="#-configuração-google">Configuração</a>
  </p>

  ![Badge em Desenvolvimento](https://img.shields.io/badge/Status-Concluído-green)
  ![License](https://img.shields.io/badge/License-MIT-blue)
</div>

---

## 📝 Sobre

O **VinilPlay** é uma aplicação web moderna de streaming de áudio que transforma o seu **Google Drive** em um servidor de música pessoal. 

Diferente de players convencionais que exigem upload prévio para um servidor específico, o VinilPlay conecta-se diretamente à API do Google, permitindo navegar pelas suas pastas, transmitir áudios em alta qualidade (MP3/FLAC) e gerenciar sua biblioteca com uma interface **Glassmorphism** futurista e responsiva.

---

## ✨ Funcionalidades

### 🎧 Experiência de Áudio
* **Streaming Direto:** Toca músicas diretamente do Google Drive sem precisar baixar o arquivo completo antes.
* **Reprodução Contínua:** Detecta automaticamente a próxima música da pasta para tocar em sequência (Auto-Next).
* **Controles Completos:** Play, Pause, Próximo, Anterior e Barra de Progresso interativa.

### 📂 Gerenciador de Arquivos (Explorer)
* **Navegação Real:** Entre e saia de pastas como no Windows Explorer/Finder.
* **Breadcrumbs:** Barra de caminho clicável para voltar rapidamente às pastas anteriores.
* **Modo de Visualização:** Altera dinamicamente entre Grid de Pastas e Lista de Músicas.
* **Upload Integrado:** Envie arquivos do seu computador direto para a pasta aberta no Drive.

### 🔐 Autenticação & Perfil
* **Login Google Seguro:** Utiliza OAuth 2.0 para garantir segurança total.
* **Persistência:** Mantém você logado mesmo se atualizar a página (Auto-Login).
* **Perfil de Usuário:** Exibe sua foto e nome do Google no canto superior.

### 🎨 UI/UX Premium
* **Design Glassmorphism:** Estética moderna com transparências, desfoques e tema Verde/Preto (Cyberpunk/Spotify vibe).
* **Modais Personalizados:** Nada de janelas feias do navegador. Alertas, confirmações e loadings são 100% estilizados.
* **Responsivo:** Funciona perfeitamente em Desktop e Mobile.

---

## 🚀 Tecnologias

Este projeto foi desenvolvido com foco em performance e Vanilla JS moderno:

* ![HTML5](https://img.shields.io/badge/HTML5-E34F26?style=flat&logo=html5&logoColor=white) **HTML5 Semântico**
* ![TailwindCSS](https://img.shields.io/badge/Tailwind_CSS-38B2AC?style=flat&logo=tailwind-css&logoColor=white) **Tailwind CSS** (Estilização rápida e responsiva)
* ![JavaScript](https://img.shields.io/badge/JavaScript-F7DF1E?style=flat&logo=javascript&logoColor=black) **JavaScript (ES6+)**
* ![Google Cloud](https://img.shields.io/badge/Google_Cloud-4285F4?style=flat&logo=google-cloud&logoColor=white) **Google Drive API v3 & Google Identity Services**

---

## 📦 Como Rodar

### Pré-requisitos

1.  Um editor de código (recomendado: **VS Code**).
2.  Extensão **Live Server** (ou qualquer servidor local).
3.  Uma conta Google.

### Passo a Passo

1.  Clone este repositório:
    ```bash
    git clone [https://github.com/seu-usuario/vinilplay.git](https://github.com/seu-usuario/vinilplay.git)
    ```
2.  Abra a pasta no VS Code.
3.  **Importante:** O Google não aceita login via arquivo direto (`file://`). Você precisa rodar em um servidor local.
    * Clique com o botão direito no `index.html` e selecione **"Open with Live Server"**.
4.  O projeto abrirá em `http://127.0.0.1:5500`.

---

## ⚙️ Configuração Google (Obrigatório)

Para que o login e o acesso ao Drive funcionem, você precisa de suas próprias chaves da API:

1.  Acesse o [Google Cloud Console](https://console.cloud.google.com/).
2.  Crie um novo projeto.
3.  Vá em **APIs & Services > Library** e ative a **Google Drive API**.
4.  Vá em **OAuth Consent Screen**:
    * Configure como "External".
    * Adicione seu e-mail em **Test Users**.
5.  Vá em **Credentials** e crie:
    * **API Key**
    * **OAuth Client ID** (Tipo: Web Application).
    * Em **Authorized Javascript Origins**, adicione: `http://127.0.0.1:5500` e `http://localhost:5500`.

6.  No código `index.html`, procure pelas variáveis e substitua:
    ```javascript
    const API_KEY = 'SUA_API_KEY_AQUI'; 
    const CLIENT_ID = 'SEU_CLIENT_ID_AQUI.apps.googleusercontent.com';
    ```

---

## 📸 Screenshots

<div align="center">
  <img src="https://via.placeholder.com/600x300?text=Tela+de+Login" alt="Login Screen" width="45%">
  <img src="https://via.placeholder.com/600x300?text=Player+e+Explorer" alt="Player Interface" width="45%">
</div>

---

## 🤝 Contribuição

Sinta-se à vontade para fazer um fork do projeto, abrir issues e enviar Pull Requests. Toda ajuda é bem-vinda para tornar o VinilPlay ainda melhor!

---

<div align="center">
  Feito com 💚 e muita música por <strong>[Seu Nome]</strong>
</div>
