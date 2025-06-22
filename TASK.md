TASK.md - Tarefas do Projeto de Blog Pessoal

Este documento rastreia as tarefas ativas, o backlog e os marcos do projeto, seguindo uma abordagem de uma tarefa por vez.

Marco 1: Fundação e Estrutura Base

Objetivo: Configurar o projeto, estilização base e criar o layout principal e o primeiro componente estático.
Marco 1: Fundação e Primeiro Deploy
    [ ] DEV-08: Criar o componente TechStack.astro com logotipos de tecnologias.


Objetivo: Ter um blog Astro básico, com o fluxo de trabalho de conteúdo funcional, implantado na Cloudflare Pages.
Tarefas Ativas

    [x] Content-04: Criar o primeiro post de teste em Markdown no Obsidian.

Backlog

    [ ] Setup-03: Criar um repositório Git privado separado para o conteúdo (meu-blog-conteudo).

    [x] Setup-04: Criar um arquivo .env.example para gerenciamento de configurações futuras.

    [ ] Deploy-01: Conectar o repositório principal do Astro à Cloudflare Pages.

    [x] Design-01: Implementar o CSS básico para a estética inspirada em café com temas Dawn e Dusk.

    [ ] Test-01: Configurar o framework de testes Vitest no projeto.

    [ ] RSS-01: Adicionar a integração @astrojs/rss para gerar o feed RSS.

    [ ] Action-01: Configurar a GitHub Action blog-post-workflow no repositório de perfil.

    [ ] DEV-01: Criar o src/layouts/BaseLayout.astro contendo a estrutura HTML base (head, body, <slot />) e importar o global.css.

    [ ] DEV-02: Implementar o script is:inline no <head> do BaseLayout.astro para carregar o tema do localStorage e prevenir o FOWT.

    [ ] DEV-03: Criar o componente Header.astro estático.

    [ ] DEV-04: Criar o componente Footer.astro estático.

    [ ] DEV-05: Criar o componente Hero.astro (título, CTAs e seta animada).

    [ ] DEV-06: Criar o componente ProjectCard.astro para exibir um único projeto.

    [ ] DEV-07: Criar a seção Portfolio.astro que renderiza uma grelha de ProjectCard.astro.

    [ ] DEV-08: Criar o componente TechStack.astro com logotipos de tecnologias.

    [ ] DEV-09: Criar o componente ExperienceCard.astro com o estilo inspirado no LinkedIn.

    [ ] DEV-10: Criar a seção Experience.astro que renderiza uma lista de ExperienceCard.astro.

    [ ] DEV-11: Criar o componente interativo ThemeToggle.astro (client:load) para a troca de temas.

Concluído

    [x] Setup-01: Inicializar um novo projeto Astro com o template de blog.
    [x] Setup-02: Criar o repositório principal no GitHub para o projeto Astro.
    [x] Content-01: Adicionar o repositório de conteúdo como um Git Submodule em src/content/blog.
    [x] Content-02: Configurar o Obsidian para usar src/content/blog como um vault.
    [x] Content-03: Instalar e configurar o plugin Obsidian Git para gerenciar commits de conteúdo.

