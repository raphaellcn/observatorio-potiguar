# Observatório do Mercado de Trabalho

Site estático para publicação dos boletins da SEPLAN/Pau dos Ferros no GitHub Pages.

## Estrutura

```text
docs/
  index.html
  boletins/
    boletim-01-caged/
    boletim-02-rais/
```

O GitHub Pages deve ser configurado para publicar a partir da pasta `docs` na branch principal.

## Como publicar no GitHub

### Opção 1: pelo Git/Git Bash

1. Crie um repositório no GitHub, por exemplo `observatorio-mt`.
2. No terminal, dentro desta pasta, rode:

```bash
git init
git add .
git commit -m "Publica site inicial dos boletins"
git branch -M main
git remote add origin https://github.com/raphaellcn/observatorio-mt.git
git push -u origin main
```

3. No GitHub, acesse `Settings > Pages`.
4. Em `Build and deployment`, selecione:

```text
Source: Deploy from a branch
Branch: main
Folder: /docs
```

5. A página ficará disponível em:

```text
https://raphaellcn.github.io/observatorio-mt/
```

### Opção 2: pelo GitHub Desktop ou upload no site

Se o comando `git` não estiver disponível no terminal, use o GitHub Desktop ou envie os arquivos pelo próprio GitHub:

1. Crie o repositório `observatorio-mt`.
2. Envie todo o conteúdo desta pasta, mantendo a pasta `docs`.
3. Configure o GitHub Pages para publicar `main` + `/docs`.

## Atualização dos boletins

Quando um boletim for atualizado, copie a nova versão HTML/PDF para a pasta correspondente em `docs/boletins/` e faça novo commit.
