# 📥 Nissin Clone

Um script para clonar canais do Telegram de forma rápida e eficiente. Com suporte para download/reenvio de mídia, criação automática de canais de destino e filtragem de mensagens por tipo.

## ✨ Funcionalidades

- 📌 Clonagem completa de mensagens de texto, mídia, vídeos, fotos, documentos, stickers, etc.
- 🚀 Modo público rápido: clona como cópia (não mostra "Encaminhado de…").
- 🧭 Download e reenvio no modo privado (permite baixar e reupar mensagens de canais privados).
- 🛡️ Sessão inteligente: reutiliza dados salvos e evita repetição de autenticação.
- 🔎 Filtros de clonagem: tudo, só texto, só mídia, só vídeo, só fotos.
- 🧩 Barra de progresso detalhada (com `tqdm`).
- 🛠️ Logs automáticos e tratamento de erros.
- 🔄 Otimização opcional de vídeos via ffmpeg (recomendado).

## 🐍 Requisitos

- Python 3.x (recomendado 3.8+)
- Bibliotecas Python:
  - telethon
  - tqdm
  - tenacity
  - aiohttp
- ffmpeg instalado no sistema (opcional, mas recomendado para vídeos).

## 🔧 Instalação

No Termux ou outro ambiente Linux/Python:

```bash
pip install telethon tqdm tenacity aiohttp
pkg install ffmpeg
```

Ou use o comando único:

```bash
pip install telethon tqdm tenacity aiohttp && pkg install ffmpeg
```

## 🚀 Como usar

1. Clone o repositório ou copie o arquivo `nissin_clone.py` para o seu diretório.
2. Rode o script:

```bash
python nissin_clone.py
```

3. Siga as instruções no terminal:
   - Escolha a sessão existente ou crie uma nova.
   - Autentique sua conta do Telegram (API ID e API Hash necessários).
   - Informe o ID do canal de origem.
   - Escolha se deseja criar automaticamente o canal de destino.
   - Escolha o modo (público rápido ou privado download/reenvio).
   - Escolha o tipo de mensagem a clonar (tudo, texto, mídia, etc.).

4. O script exibirá logs detalhados durante a clonagem.

## ⚠️ Observações

- O Telegram limita a quantidade de mensagens e mídias que podem ser encaminhadas ou reenviadas rapidamente. Use com moderação para evitar limites de spam.
- Para canais privados, é necessário usar o modo download/reenvio (privado).
- O script não contorna restrições de API ou políticas do Telegram. Use por sua conta e risco.

## 📜 Licença

MIT License
