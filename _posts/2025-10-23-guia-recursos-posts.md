---
layout: post
title: "Guia de Uso: Recursos dos Posts"
date: 2025-10-23 09:00:00 -0300
categories: [Tutorial]
tags: [guia, tutorial, jekyll]
description: "Aprenda a usar todos os recursos disponíveis nos posts deste site"
author: Carlos Costa
reading_time: "5 min de leitura"
hero_image: /images/posts/jekyll-tutorial/tutorial-hero.jpg
---

## Bem-vindo!

Este post demonstra todos os recursos disponíveis no layout de posts. Todos esses recursos já estão **ATIVOS POR PADRÃO** - você não precisa configurar nada no front matter!

## Recursos Automáticos

Quando você cria um post, os seguintes recursos já estão funcionando:

- 🌙 **Dark/Light Mode** - Botão no topo da página
- 🔤 **Controle de Fonte** - Botões A+ e A- para ajustar tamanho
- 📈 **Barra de Progresso** - Mostra quanto você já leu
- 📋 **Índice Flutuante** - Botão ☰ abre o índice do artigo
- 🔍 **Lightbox** - Clique em qualquer imagem para dar zoom
- ↑ **Voltar ao Topo** - Botão que aparece ao rolar a página
- 💌 **Animações** - Elementos aparecem suavemente ao rolar

{% include post-boxes.html 
   type="info" 
   title="Informação Importante" 
   content="Você NÃO precisa adicionar `enable_dark_mode: true` ou similares no front matter. Todos os recursos já são PADRÃO!" 
%}

## Caixas Especiais

Você pode usar vários tipos de caixas para destacar conteúdo. Veja exemplos:

### Caixa de Destaque

{% include post-boxes.html 
   type="highlight" 
   title="💡 Destaque" 
   content="Use esta caixa para destacar informações importantes ou insights principais." 
%}

### Caixa de Citação

{% include post-boxes.html 
   type="quote" 
   title="Frase Inspiradora" 
   content="A única maneira de fazer um ótimo trabalho é amar o que você faz." 
   author="Steve Jobs" 
%}

### Caixa de Aviso

{% include post-boxes.html 
   type="warning" 
   title="Atenção" 
   content="Use esta caixa para avisos importantes que requerem atenção especial do leitor." 
%}

### Caixa de Sucesso

{% include post-boxes.html 
   type="success" 
   title="Parabéns!" 
   content="Você completou esta seção com sucesso! Use esta caixa para mensagens positivas." 
%}

### Caixa de Exemplo

{% include post-boxes.html 
   type="example" 
   title="Exemplo Prático" 
   content="Esta é uma caixa ideal para demonstrações e exemplos práticos de conceitos." 
%}

### Caixa de Definição

{% include post-boxes.html 
   type="definition" 
   title="Definição: Jekyll" 
   content="Jekyll é um gerador de sites estáticos escrito em Ruby, ideal para blogs e sites de documentação." 
%}

### Caixa de Nota

{% include post-boxes.html 
   type="note" 
   title="Nota" 
   content="Use esta caixa para observações adicionais ou notas de rodapé." 
%}

### Curiosidade

{% include post-boxes.html 
   type="fun-fact" 
   title="Você Sabia?" 
   content="O Jekyll foi criado por Tom Preston-Werner, co-fundador do GitHub, e é usado para hospedar milhões de sites no GitHub Pages!" 
%}

## Grade de Conceitos

Para exibir múltiplos conceitos relacionados lado a lado:

{% include post-boxes.html type="concept-grid-start" %}

{% include post-boxes.html 
   type="concept" 
   title="Conceito 1" 
   content="Primeira ideia ou conceito importante" 
%}

{% include post-boxes.html 
   type="concept" 
   title="Conceito 2" 
   content="Segunda ideia ou conceito relacionado" 
%}

{% include post-boxes.html 
   type="concept" 
   title="Conceito 3" 
   content="Terceira ideia para completar a visão geral" 
%}

{% include post-boxes.html type="concept-grid-end" %}

## Linha do Tempo (Timeline)

Perfeita para mostrar eventos cronológicos:

{% include post-boxes.html type="timeline-start" %}

{% include post-boxes.html 
   type="timeline-item" 
   year="2008" 
   title="Criação do Jekyll" 
   content="Tom Preston-Werner lança a primeira versão do Jekyll." 
%}

{% include post-boxes.html 
   type="timeline-item" 
   year="2013" 
   title="Jekyll 1.0" 
   content="Lançamento da versão 1.0 com melhorias significativas." 
%}

{% include post-boxes.html 
   type="timeline-item" 
   year="2025" 
   title="Uso Atual" 
   content="Jekyll continua sendo uma das ferramentas mais populares para sites estáticos." 
%}

{% include post-boxes.html type="timeline-end" %}

## Pergunta Final

Use esta caixa especial para encerrar o post com uma reflexão:

{% include post-boxes.html 
   type="final-question" 
   title="Pense nisso..." 
   content="Agora que você conhece todos os recursos, que tipo de conteúdo incrível você vai criar?" 
%}

## Como Usar

Para usar qualquer caixa, basta copiar e colar este código no seu post:

```liquid
{% raw %}{% include post-boxes.html 
   type="info" 
   title="Título da Caixa" 
   content="Seu conteúdo aqui" 
%}{% endraw %}
```

### Tipos Disponíveis:

- `highlight` - Destaque
- `quote` - Citação (pode usar `author="Nome"`)
- `warning` ou `danger` - Aviso
- `info` - Informação
- `success` - Sucesso
- `example` - Exemplo
- `definition` - Definição
- `note` - Nota
- `fun-fact` - Curiosidade
- `final-question` - Pergunta final

### Para Grade de Conceitos:

```liquid
{% raw %}{% include post-boxes.html type="concept-grid-start" %}

{% include post-boxes.html 
   type="concept" 
   title="Título" 
   content="Descrição" 
%}

{% include post-boxes.html type="concept-grid-end" %}{% endraw %}
```

### Para Timeline:

```liquid
{% raw %}{% include post-boxes.html type="timeline-start" %}

{% include post-boxes.html 
   type="timeline-item" 
   year="2025" 
   title="Evento" 
   content="Descrição" 
%}

{% include post-boxes.html type="timeline-end" %}{% endraw %}
```

## Front Matter Simplificado

Você só precisa destes campos no início do post:

```yaml
---
layout: post
title: "Título do Post"
date: 2025-10-23
categories: [Categoria]
tags: [tag1, tag2]
description: "Descrição para SEO"
author: Carlos Costa
reading_time: "5 min de leitura"
hero_image: /images/posts/pasta/imagem.jpg  # Opcional
---
```

**IMPORTANTE:** Você NÃO precisa adicionar:
- `enable_dark_mode: true`
- `enable_toc: true`
- `enable_lightbox: true`
- Etc.

**Todos esses recursos já são PADRÃO!**

{% include post-boxes.html 
   type="success" 
   title="Pronto para Começar!" 
   content="Agora você tem tudo que precisa para criar posts incríveis. Divirta-se criando conteúdo!" 
%}
