# PoE Rush Overlay

Programa para auxiliar em **Rush de leveling no Path of Exile 2**. Um painel
overlay in-game que registra automaticamente os compradores e organiza os
atendimentos enquanto você joga.

<p align="center">
  <a href="https://github.com/falvstech/rush-overlay-dist/releases/latest"><img src="https://img.shields.io/github/v/release/falvstech/rush-overlay-dist?label=vers%C3%A3o&color=c8a657" alt="Última versão"></a>
  <a href="https://github.com/falvstech/rush-overlay-dist/releases"><img src="https://img.shields.io/github/downloads/falvstech/rush-overlay-dist/total?label=downloads&color=7bbf6a" alt="Downloads"></a>
  <img src="https://img.shields.io/badge/plataforma-Windows-2d6fb0" alt="Plataforma Windows">
</p>

<p align="center">
  <img src="docs/rush.png" alt="Tela de rush do overlay com clientes de exemplo" width="320">
</p>

## Download e instalação

<p align="center">
  <a href="https://github.com/falvstech/rush-overlay-dist/releases/latest"><img src="https://img.shields.io/badge/⬇%20Baixar%20instalador-c8a657?style=for-the-badge&logoColor=black" alt="Baixar instalador"></a>
</p>

Ou baixe o `RushOverlay-Setup-x.y.z.exe` direto na página de
**[Releases](https://github.com/falvstech/rush-overlay-dist/releases/latest)**,
execute e siga o assistente. **Não precisa de Python nem de nada instalado** — o
app é standalone.

O instalador coloca o app em `Program Files (x86)` e cria atalho na Área de
Trabalho e no Menu Iniciar.

> **Requisito:** PoE 2 em modo **Janela** ou **Janela sem borda** (fullscreen
> exclusivo cobre o overlay).

## O que faz

- Whisper `Leveling carry (X to Y)` → registra **nome + faixa de level + preço**
  (pela tabela). Aceita variações (`1 to 70`, `1-70`, `1 a 70`) e cliente EN
  (`@From`) / BR (`@De`).
- Até **4 clientes simultâneos** + fila de espera para os próximos.
- Botão **convidar** copia `/invite Nome` e envia no chat do jogo.
- Timer por cliente, dropdown de classe e ações de concluir / cancelar /
  antecipado / pagar / prorrogar.
- **Comunicação:** sussurra direto pro comprador ou dispara mensagens-modelo.

## Abas

- **RUSH** — clientes ativos.
- **PREÇOS** — tabela editável faixa → div (recalcula os ativos ao salvar).
- **CONFIG** — hotkey (padrão `ctrl+d`), caminho do `Client.txt`
  (auto-detecta Steam/standalone), regex do whisper e opacidade.

## Pin / mouseover

Botão de tachinha no topo alterna entre **fixo** (painel sempre visível) e
**hover** (colapsa numa barra fina e expande ao passar o mouse).

## Problemas comuns

- **Hotkey não funciona com o jogo em foco** → execute como Administrador (o
  jogo elevado bloqueia hooks de apps não elevados).
- **"log NÃO encontrado"** → na aba CONFIG, aponte o `Client.txt`
  (`.../Path of Exile 2/logs/Client.txt`).
