---
layout: post
title: "Construindo seu Primeiro Site com Jekyll"
date: 2025-10-18 09:00:00 -0300
categories: [Programação, Web]
tags: [jekyll, ruby, web, tutorial]
description: "Aprenda a criar um site estático moderno usando Jekyll e GitHub Pages"
author: Carlos Costa
reading_time: "15 min de leitura"
image: /images/blog/default-post.jpg
---

## Por Que Jekyll?

Jekyll é um gerador de sites estáticos que transforma arquivos de texto simples em sites completos. É perfeito para blogs, portfólios e documentação.

## Pré-requisitos

Antes de começar, certifique-se de ter:

- Ruby instalado (versão 2.5 ou superior)
- RubyGems
- GCC e Make

## Instalando o Jekyll

```bash
gem install jekyll bundler
```

## Criando seu Primeiro Site

```bash
jekyll new meu-site
cd meu-site
bundle exec jekyll serve
```

Acesse `http://localhost:4000` para ver seu site!

## Estrutura de Pastas

- `_posts/`: Seus artigos do blog
- `_layouts/`: Templates HTML
- `_includes/`: Componentes reutilizáveis
- `_config.yml`: Configurações do site
- `assets/`: CSS, JavaScript e imagens

## Escrevendo Posts

Crie arquivos em `_posts/` com o formato:

```
AAAA-MM-DD-titulo-do-post.md
```

## Personalizando seu Site

Edite o `_config.yml` para personalizar:

- Título do site
- Descrição
- URL base
- Tema

## Deploy no GitHub Pages

1. Crie um repositório no GitHub
2. Faça push do código
3. Ative o GitHub Pages nas configurações

Seu site estará online em minutos!

## Conclusão

Jekyll é uma ferramenta poderosa e simples para criar sites estáticos. Experimente e divirta-se criando!