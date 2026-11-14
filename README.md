# 🏠 NewHouse Quixadá — Plataforma de Moradia Estudantil

Plataforma digital voltada para conectar estudantes universitários (UFC, UECE, IFCE, Unicatólica) e proprietários de imóveis em **Quixadá - CE**, oferecendo busca inteligente por raio e estilo de vida, agendamento de visitas, vistoria digital, contratos eletrônicos e sistema de reputação mútua.

Projeto desenvolvido para a disciplina de **Engenharia de Requisitos** (Universidade Federal do Ceará — Campus Quixadá).

---

## 🔗 Protótipo Navegável de Alta Fidelidade (Figma)

Explore os fluxos completos de **Estudante**, **Proprietário** e **Moderação Administrativa** diretamente no protótipo interativo:

👉 **[Acessar Protótipo Interativo no Figma](https://www.figma.com/proto/W5SDw7f3bQJguUdqsxnVRQ/Untitled?node-id=2-4&p=f&viewport=-13824%2C-98%2C1&t=Q1HLUkkkxsM8pMQU-1&scaling=min-zoom&content-scaling=fixed&page-id=0%3A1)**

---

## ✨ Principais Funcionalidades

* **Autenticação e Onboarding em 3 Etapas (`RNF001`):** Cadastro diferenciado para estudantes e proprietários com validação de vínculo acadêmico e preferências de convivência.
* **Catálogo e Filtros Inteligentes (`RF010` / `RF011`):** Busca filtrada por raio de distância até o campus, faixa de preço, contas inclusas e compatibilidade de estilo de vida.
* **Favoritos e Comparação Lado a Lado:** Salvamento de imóveis de interesse com matriz comparativa de valores, infraestrutura e distância.
* **Comunicação Síncrona e Negociação:** Chat direto entre estudante e proprietário integrado ao contexto do anúncio.
* **Agendamento de Visitas (`RF014`):** Solicitação de visitas presenciais ou por videochamada com seleção de data e horário.
* **Gestão de Imóveis e Quartos (`RF008`):** Cadastro composto de imóveis e quartos individuais/compartilhados, controle de regras do local e opção rápida para pausar anúncios alugados.
* **Vistoria Digital e Contratos (`RF017`):** Checklist de entrada/saída com registro fotográfico e formalização de contrato digital com assinatura eletrônica.
* **Reputação Bidirecional (`RF019`) e Moderação (`RF020`):** Avaliação mútua pós-locação (estudante $\leftrightarrow$ proprietário) e painel administrativo para validação de documentos, aprovação de anúncios e tratamento de denúncias.

---

## 🎨 Design System & Acessibilidade

O protótipo foi refinado seguindo padrões rigorosos de UI/UX:
* **Dark Mode de Alto Contraste (WCAG AA/AAA):** Fundo principal em `#0F172A` (Slate 900), superfícies em `#1E293B` (Slate 800) e tipografia em `#F8FAFC` com taxa de contraste superior a **7:1**.
* **Grid e Responsividade:** Estrutura adaptada para **Mobile (`390×844px`, grid de 4 colunas)** e **Desktop (`1440×900px`, grid de 12 colunas)**, garantindo navegação fluida em até 3 cliques (`RNF002`).

---

## 🏗️ Arquitetura e Stack Tecnológica Planejada

| Camada | Tecnologias |
| :--- | :--- |
| **Front-end** | React / Next.js (TypeScript) + Tailwind CSS |
| **Back-end** | Node.js (NestJS) |
| **Banco de Dados & Cache** | PostgreSQL + Redis (SLA de busca $< 2,0\text{s}$ — `RNF003`) |
| **Tempo Real** | WebSockets (Socket.io) |
| **Segurança & LGPD** | HTTPS / TLS 1.3 e hashing Argon2id (`RNF001`) |
