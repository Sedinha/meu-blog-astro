Projeto de Blog Pessoal Automatizado com Astro e Obsidian

Este repositório contém o código-fonte e a arquitetura para um blog pessoal moderno e de alta performance, projetado para maximizar a marca pessoal de um desenvolvedor através de um fluxo de trabalho de conteúdo altamente automatizado.

O projeto é construído sobre a filosofia "Content as Code" e segue uma metodologia de desenvolvimento assistida por IA rigorosa para garantir um código limpo, modular e escalável.
Visão Geral da Arquitetura

O projeto integra um conjunto de ferramentas modernas para criar um ciclo virtuoso de criação e distribuição de conteúdo:

    Escrita (IDE de Conteúdo): Obsidian é usado para criar e gerenciar todo o conteúdo em arquivos .md locais.

    Repositório de Conteúdo: Um repositório Git separado (Git Submodule) contém todos os artigos, desacoplando o conteúdo da sua apresentação.

    Site (Camada de Apresentação): Um projeto Astro consome os arquivos Markdown para gerar um site estático, rápido e otimizado para SEO, com uma estética de pixel art.

    Hospedagem e CI/CD: A Cloudflare Pages realiza o deploy contínuo, oferecendo uma rede de entrega global de alta performance.

    Automação da Marca: Uma GitHub Action monitora o feed RSS do blog e atualiza dinamicamente a seção de artigos no README do perfil do GitHub.

Princípios de Desenvolvimento

Este projeto é gerenciado com o auxílio de uma IA e segue um conjunto estrito de regras para garantir a qualidade:

    Gerenciamento por Markdown: O escopo é definido no PLANNING.md e as tarefas no TASK.md.

    Modularidade: Os arquivos de código são mantidos concisos (idealmente < 200 linhas) e organizados por responsabilidade.

    Testes: Novos recursos são acompanhados por testes para garantir a confiabilidade.

    Especificidade: As interações com a IA são focadas em uma única tarefa por vez para garantir a precisão.

Para entender a visão completa, a arquitetura e os próximos passos, consulte os seguintes documentos:

    PLANNING.md: Contém a visão de alto nível do projeto, as decisões de arquitetura e os princípios de desenvolvimento.

    TASK.md: Detalha a lista de tarefas atuais, o backlog e os marcos para o desenvolvimento.