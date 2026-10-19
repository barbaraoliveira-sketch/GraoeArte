# Grão & Arte - Torrefação e Café Especial ☕

## 1. Visão Geral e Objetivo do Projeto
O **Grão & Arte** é uma plataforma web desenvolvida para apresentar uma torrefação artesanal de cafés especiais. O objetivo do projeto é conectar pequenos produtores diretos a apreciadores de cafés 100% Arábica de alta pontuação (SCA > 85 pts), oferecendo um catálogo de microlotes exclusivos, informações detalhadas sobre o processo de torra e um clube de assinatura mensal[cite: 3, 6, 7].

O projeto foi construído para simular um ambiente de desenvolvimento front-end profissional[cite: 1], priorizando:
- Layout fluido e adaptável a diferentes dispositivos.
- Acessibilidade e boas práticas de semântica HTML5[cite: 1].
- Separação rigorosa de responsabilidades e arquitetura de código limpa[cite: 1, 2].

---

## 2. Tecnologias e Conceitos Aplicados

- **HTML5 Semântico:** Utilização de tags apropriadas (`<header>`, `<nav>`, `<main>`, `<section>`, `<article>`, `<details>`, `<summary>`, `<footer>`) para garantir acessibilidade e SEO[cite: 1, 3, 4, 8].
- **CSS3 / Design System:**
  - **Variáveis CSS (`:root`):** Padronização de cores, tipografia, bordas, sombras e tempos de transição[cite: 4, 5].
  - **Metodologia BEM (Block Element Modifier):** Convenção de nomenclatura de classes para maior manutenibilidade do CSS.
  - **Flexbox:** Organização e alinhamento do layout de cards e seções[cite: 3].
  - **Escala REM e Unidades Relativas:** Uso do elemento raiz (`html`) ajustado percentualmente e uso de `rem` para tipografia, espaçamentos e bordas, preservando a acessibilidade das preferências do navegador[cite: 2].
  - **Unidades de Visualização (`vh`, `vw`, `%`):** Aplicação de porcentagens em containers e `vh`/`vw` para controle de seções em tela cheia[cite: 2].
- **Google Fonts:** Importação e integração das famílias `Merriweather` (títulos) e `Open Sans` (corpo de texto)[cite: 2, 5].
- **APIs & Recursos Externos:** Integração com a API do WhatsApp para contato direto e inclusão de imagens via serviços de placeholders/bancos de imagens integrados[cite: 2, 4].

---

## 3. Organização da Arquitetura de Arquivos

```text
grao-e-arte/
├── assets/
│   ├── images/          # Imagens e recursos visuais do projeto
│   └── icons/           # Ícones utilizados
├── css/
│   ├── variables.css    # Tokens globais do Design System (Cores, Fontes, Sombras)
│   ├── global.css       # Resets, regra raiz da escala REM e estilos genéricos
│   ├── components.css   # Estilos BEM dos componentes (Cards, Botões, FAQ)
│   └── layout.css       # Estilização do Header fixo, Sections, Flexbox e Footer fixo
├── index.html           # Documento principal da aplicação
└── README.md            # Documentação técnica do projeto