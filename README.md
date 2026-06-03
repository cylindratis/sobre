# Atualização do site

Arquivos principais neste pacote:

- `index.html`
- `sobre-nos/index.html`
- `_layouts/post.html`
- `_authors/adriane-borges.md`
- `_config_autores_snippet.yml`

## O que mudou

- "Autores" virou "Sobre nós".
- A página "Sobre nós" tem um parágrafo do manifesto.
- Autores não têm mais páginas individuais.
- Autores aparecem como cards com nome, descrição breve e ícones: X, Lattes e email.
- A página inicial teve a hero reduzida para os supercards aparecerem um pouco.
- O menu foi padronizado: Início, Acervo, Sobre nós, Manifesto.
- O rodapé foi homogeneizado com logo, copyright, toggle claro/escuro e menu.
- O Acervo ganhou texto explicativo, busca textual e filtro por autor.

## Atualização do `_config.yml`

Use o conteúdo de `_config_autores_snippet.yml`.

```yaml
collections:
  authors:
    output: false
```

## Como adicionar autor

Crie um arquivo em `_authors/`, por exemplo:

```text
_authors/nome-do-autor.md
```

Modelo:

```markdown
---
name: Nome do Autor
title: Nome do Autor
role: Editoria
order: 2
description: "Breve descrição do autor."
short_bio: "Breve descrição do autor."
x_url: "https://x.com/usuario"
lattes_url: "http://lattes.cnpq.br/0000000000000000"
email: "email@dominio.com"
---

Conteúdo interno opcional.
```

## Atenção

Se existir a pasta antiga `autores/`, você pode remover ou deixar redirecionando para `/sobre-nos/`.
