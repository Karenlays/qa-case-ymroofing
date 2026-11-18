# 🔍 Case de QA & Testes Exploratórios — VIZUH (ymroofing.com)

> [!NOTE]
> **Status da Aplicação:** As inconsistências relatadas neste estudo de caso já foram corrigidas pela equipe de desenvolvimento em produção. As evidências visuais anexadas na pasta `docs/assets/` ilustram os pontos auditados após a validação das correções (reteste).

> **Resumo do Projeto:** Relatório técnico de Quality Assurance (QA) e testes exploratórios desenvolvidos no escopo de entregas da **VIZUH**. O foco da auditoria foi a validação de interface, responsividade, comportamento de *breakpoints* e usabilidade em múltiplos dispositivos para a aplicação web `ymroofing.com`.

---

## 🎯 Objetivo da Auditoria
Garantir a estabilidade visual e funcional das interfaces web antes da liberação para o cliente final, identificando falhas de dimensionamento em resoluções variadas, sobreposição de elementos flutuantes e pontos de melhoria na experiência do usuário (UX).

---

## 🛠️ Metodologia e Escopo
* **Contexto Profissional:** Atuação como estagiária e colaboradora na **VIZUH**.
* **Abordagem:** Testes exploratórios baseados em fluxos reais de navegação e inspeção de elementos de front-end via DevTools.
* **Foco da Análise:**
  * Responsividade da *Hero Section* e blocos de conteúdo estrutural.
  * Comportamento de quebra de linha em *breakpoints* de transição (Desktop, Tablet e Mobile).
  * Posicionamento e sobreposição de componentes fixos/flutuantes (ex: botões de contato).

---

## 📋 Cenários de Teste & Relatório de Inconsistências

| ID do Cenário | Módulo / Funcionalidade | Descrição do Cenário (O que foi testado) | Comportamento Esperado | Status da Correção |
| :---: | :--- | :--- | :--- | :--- |
| **CT-01** | Responsividade de Layout | Validação do comportamento da página principal em larguras de tela dinâmicas. | Os blocos de conteúdo e imagens principais devem se redimensionar fluidamente sem distorções no grid. | 🟢 **Corrigido pelo time de Dev** |
| **CT-02** | Breakpoints de Exibição | Verificação de margens e seções em resoluções de transição intermediárias. | Elementos visuais devem manter espaçamentos proporcionais sem sobreposições indesejadas. | 🟢 **Corrigido pelo time de Dev** |
| **CT-03** | Elementos de Interface (UI) | Análise de posicionamento de botões fixos de chamada para ação (CTA). | Componentes flutuantes devem respeitar as camadas da tela sem obstruir a leitura de textos críticos. | 🟢 **Corrigido pelo time de Dev** |

---

## 🔄 Ciclo de Vida do Bug (Feedback Loop)
1. **Identificação:** Execução de testes exploratórios e mapeamento das inconsistências visuais nas telas do projeto.
2. **Reporte Técnico:** Documentação e alinhamento dos pontos críticos com a equipe de desenvolvimento da **VIZUH**.
3. **Validação de Correção (Reteste):** Homologação pós-deploy confirmando que os elementos ajustados atenderam aos critérios de estabilidade e responsividade.

---

## 🔒 Próximos Passos & Evolução
* [ ] Implementação de rotinas de validação de schema e sanitização em formulários de contato.
* [ ] Introdução de automação de testes E2E focados em regressão visual.

---

## 👩‍💻 Autoria
Desenvolvido por **Karen Laís Lima Gualberto** — Engenharia de Software | Quality Assurance (QA) & Cibersegurança.
Desenvolvido por **Karen Laís Lima Gualberto** — Engenharia de Software | Quality Assurance (QA) & Cibersegurança.
