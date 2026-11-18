# 🔍 Case de QA & Análise Exploratória — ymroofing.com

> **Resumo do Projeto:** Relatório técnico de Quality Assurance (QA) focado em testes exploratórios, validação de responsividade, quebra de *breakpoints* e sobreposição de elementos em múltiplos dispositivos para a aplicação web `ymroofing.com`.

---

## 🎯 Objetivo da Análise
Identificar inconsistências visuais, falhas de adaptação em diferentes resoluções de tela (desktop, tablet e mobile) e pontos de melhoria na experiência do usuário (UX) e segurança de formulários, garantindo maior estabilidade para a interface.

---

## 🛠️ Metodologia e Ferramentas
* **Técnica:** Testes exploratórios manuais baseados em cenários de uso real.
* **Ferramentas:** Chrome DevTools (Device Mode, Responsive View, Network & Console).
* **Foco da Varredura:** 
  * Responsividade da *Hero Section* e blocos de conteúdo[span_4](start_span)[span_4](end_span).
  * Comportamento de *breakpoints* em telas intermediárias e largas[span_5](start_span)[span_5](end_span).
  * Posicionamento de elementos flutuantes (*z-index* e sobreposição)[span_6](start_span)[span_6](end_span)[span_7](start_span)[span_7](end_span).
  * Validação de sanitização e prevenção de vulnerabilidades (ex: XSS) em formulários[span_8](start_span)[span_8](end_span).

---

## 📋 Tabela de Inconsistency / Relatório de Bugs

| ID | Funcionalidad/Módulo | Descrição do Problema | Dispositivo / Resolução | Status |
| :---: | :--- | :--- | :--- | :--- |
| **01** | Responsividade (Hero / Blocos) | Cortes inadequados e falhas de renderização nos blocos laterais e imagens principais. | Desktop / Responsivo[span_9](start_span)[span_9](end_span)[span_10](start_span)[span_10](end_span) | 🔴 Aberto |
| **02** | Breakpoints de Exibição | Elementos visuais falham ao se adaptar em escalas de transição (ex: desalinhamento de seções e margens). | Desktop & Tablet[span_11](start_span)[span_11](end_span)[span_12](start_span)[span_12](end_span) | 🔴 Aberto |
| **03** | Sobreposição de Elementos | O botão flutuante de contato fica posicionado por cima dos cards de serviços, prejudicando a leitura. | Mobile / Responsivo[span_13](start_span)[span_13](end_span)[span_14](start_span)[span_14](end_span) | 🔴 Aberto |

---

## 📸 Evidências Técnicas (Prints de Validação)

### Evidência 01: Falha de renderização nos blocos de conteúdo
> ![Bug de Blocos](./docs/assets/bug-01-blocos.jpg)  
> *Descrição:* Elementos e blocos laterais apresentando falhas de dimensionamento no modo responsivo[span_15](start_span)[span_15](end_span)[span_16](start_span)[span_16](end_span).

### Evidência 02: Desalinhamento em breakpoints de transição
> ![Bug de Breakpoints](./docs/assets/bug-02-breakpoints.jpg)  
> *Descrição:* Margens e seções sofrendo cortes e sobreposições nas larguras intermediárias[span_17](start_span)[span_17](end_span)[span_18](start_span)[span_18](end_span).

### Evidência 03: Botão flutuante sobrepondo o conteúdo
> ![Bug de Sobreposição](./docs/assets/bug-03-sobreposicao.jpg)  
> *Descrição:* O botão fixo de ligação cobre textos críticos dos cards de serviços (`Residential / Commercial`)[span_19](start_span)[span_19](end_span)[span_20](start_span)[span_20](end_span).

---

## 🔒 Próximos Passos (Evolução para AppSec)
* [ ] Validação de schema no front-end para evitar submissões incorretas.
* [ ] Execução de testes de injeção e sanitização (prevenção contra XSS) no formulário de contato[span_21](start_span)[span_21](end_span).
* [ ] Implementação de automação de testes E2E com Playwright para regressão visual.

---

## 👩‍💻 Autoria
Desenvolvido por **Karen Laís Lima Gualberto** — Engenharia de Software | Quality Assurance (QA) & Cibersegurança.
