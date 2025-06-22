Projeto de Blog Pessoal Automatizado com Astro e Obsidian

Este repositório contém o código-fonte e a arquitetura para um blog pessoal moderno e de alta performance, projetado para maximizar a marca pessoal de um desenvolvedor através de um fluxo de trabalho de conteúdo altamente automatizado. Construído com um fluxo de trabalho moderno que integra Astro.js para performance, Tailwind CSS para estilização e é desenvolvido com o auxílio de assistentes de IA (v0.dev + LLM na IDE).

O projeto visa criar uma identidade de marca forte, com uma estética minimalista inspirada em tons de café, e serve como uma vitrine para projetos, experiências e artigos.

Visão Geral da Arquitetura

    Framework: Astro.js - Focado em conteúdo, performance (Zero-JS por padrão) e excelente experiência de desenvolvimento.

    Estilização: Tailwind CSS - Framework de utilitários para criar designs customizados rapidamente.

    Geração de Componentes de UI: v0.dev - Usado para gerar o boilerplate de componentes React + Tailwind, que são então adaptados para o Astro.

    Sistema de Temas: Implementação de múltiplos temas (ex: Dawn, Dusk) com variáveis CSS e um seletor de tema dinâmico que persiste a escolha do usuário.

    Estrutura: O site é composto por seções modulares e reutilizáveis, como Herói, Portfólio, Tecnologias e Experiências.

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

    Desenvolvimento Assistido por IA

Este projeto é gerenciado com uma metodologia estrita para garantir a qualidade e a organização do código ao colaborar com IAs.

    PLANNING.md: Contém a visão de alto nível, as decisões de arquitetura, a pilha de tecnologia e os princípios de design. A IA deve consultá-lo para entender o contexto do projeto.

    TASK.md: Detalha a lista de tarefas ativas, o backlog e os marcos do desenvolvimento. É o guia da IA para a próxima ação a ser executada.

    AI_GLOBAL_RULES.md: Um conjunto de regras que a IA deve seguir estritamente durante todo o ciclo de desenvolvimento.

Para começar, explore os arquivos de planejamento e tarefas para entender o escopo completo.