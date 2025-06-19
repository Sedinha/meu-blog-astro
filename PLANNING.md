PLANNING.md - Visão do Projeto de Blog Pessoal
1. Propósito e Visão de Alto Nível

O objetivo deste projeto é construir uma plataforma de publicação de conteúdo pessoal que sirva como ferramenta de autopromoção e reforço de marca para um desenvolvedor de software, seguindo a filosofia "Content as Code" e uma metodologia de desenvolvimento estruturada.

O ciclo virtuoso desejado é: Escrever no Obsidian -> Commit & Push -> Deploy Automático -> Distribuição via RSS -> Atualização Automática do Perfil do GitHub.
2. Arquitetura do Sistema

    Fonte da Verdade do Conteúdo: Um repositório Git privado, gerenciado como um Git Submodule.

    Camada de Apresentação: Um projeto Astro que consome o conteúdo do submódulo.

    Integração de Conteúdo: O submódulo de conteúdo será localizado em src/content/blog.

    Implantação e CI/CD: Cloudflare Pages, acionada por git push no repositório principal.

    Automação de Perfil: Feed RSS gerado pelo Astro para alimentar uma GitHub Action.

3. Pilha de Tecnologia (Tech Stack) e Ferramentas

Componente
	

Ferramenta Escolhida
	

Justificativa

Framework do Site
	

Astro
	

Performance (Zero-JS por padrão), focado em conteúdo e ótima DX.

Ambiente de Escrita
	

Obsidian
	

"IDE para Markdown" que funciona com arquivos locais, compatível com Git.

Controle de Versão
	

Git / GitHub
	

Padrão da indústria, essencial para "Content as Code".

Integração de Conteúdo
	

Git Submodules
	

Desacopla conteúdo do código, permitindo versionamento independente.

Hospedagem e CI/CD
	

Cloudflare Pages
	

Plano gratuito robusto e suporte nativo a Git Submodules.

Automação de Perfil
	

GitHub Actions (blog-post-workflow)
	

Solução nativa e popular para agregar feeds RSS.

Estilo e Design
	

CSS customizado / Tailwind CSS
	

Implementação de estética minimalista com pixel art. Tailwind para utilitários.

Testes
	

Vitest
	

Framework de testes moderno e rápido, com ótima integração com o Vite (usado pelo Astro).
4. Princípios e Regras de Desenvolvimento

    Arquivos Concisos: Nenhum arquivo de código deve exceder 200-500 linhas. Refatorar em módulos menores quando necessário.

    Nomenclatura Descritiva: Usar nomes de arquivos em kebab-case.ts e nomes de funções/variáveis extremamente descritivos (ex: fetchRecentBlogPostsFromRssFeed). Evitar abreviações.

    Estrutura de Diretórios: Organizar os diretórios por responsabilidade (ex: src/components, src/layouts, src/utils, src/services).

    Testes: Sempre criar testes unitários para novas funcionalidades. Escrever funções puras sempre que possível para facilitar os testes.

    Segurança: Todas as chaves, segredos e configurações devem ser gerenciados em um arquivo .env, com um .env.example para referência.

    Comentários: Os comentários no código devem ser em Inglês e explicar o "porquê" de uma decisão, não o "como" o código funciona.