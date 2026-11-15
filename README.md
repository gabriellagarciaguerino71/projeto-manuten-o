# Sistema Automatizado de Extração e Controle de Calibração
> **Modelagem Conceitual e Gestão de Riscos Operacionais em Esteira Cloud, IA e OCR**

---

## 👥 Equipe de Desenvolvimento
* **Victória Maria**
* **Gabriella**
* **Ana Carolinne**

---

## 📌 Visão Geral & Contexto Operacional
Nas plantas industriais modernas, a calibração periódica de instrumentos e sensores (manômetros, paquímetros, transmissores de pressão e temperatura) é executada por empresas metrológicas terceirizadas credenciadas, emitindo laudos em formato PDF digital.

Atualmente, o processo de conferência e inserção dessas informações no sistema de gestão é realizado manualmente pela equipe da Qualidade, gerando gargalos críticos:
* **Risco de Falhas Humanas:** Digitação mecânica de sequências numéricas longas e casas decimais metrológicas.
* **Desperdício de Horas Técnicas:** Cerca de 100 horas mensais dedicadas a tarefas repetitivas.
* **Atraso Gerencial:** Dados vitais represados nos PDFs, retardando tomadas de decisão para a Manutenção Preventiva.

O presente projeto propõe a **modelagem conceitual e lógica de uma esteira automatizada** que captura os laudos em nuvem corporativa (OneDrive/SharePoint), executa a extração automatizada de dados via motor OCR assistido por IA e valida as leituras antes da gravação no banco de dados.

---

## ⚠️ Delimitação e Restrição de Escopo
* **Natureza Conceitual:** Trabalho puramente de modelagem teórica, mapeamento de fluxos AS-IS / TO-BE, especificação de requisitos de engenharia de software e gestão de riscos operacionais.
* **Restrição Absoluta:** O projeto **NÃO contempla programação prática, codificação de software executável ou implantação em ambiente real de produção operacional**.

---

## ⚙️ Arquitetura Lógica da Solução (3 Passos)
1. **Passo 01 — Entrada de Arquivos:** Os certificados recebidos são depositados em pasta monitorada em nuvem corporativa (OneDrive / SharePoint).
2. **Passo 02 — Extração Inteligente:** Disparo automático de pipeline com pré-processamento de imagem (OpenCV/Otsu), OCR e inteligência artificial para captura de campos críticos (vigência, instrumentos, faixas e erros).
3. **Passo 03 — Validação e Consolidação:** Camada lógica de regras metrológicas (*Business Rules Engine*) que verifica consistência estatística de tolerâncias e consolida os dados na base em nuvem.

---

## 📁 Documentos Oficiais de Gestão do Projeto (/docs)
Os relatórios formais desenvolvidos segundo as diretrizes do PMBOK e da disciplina estão arquivados na pasta `/docs`:

| Arquivo | Descrição Principal |
| :--- | :--- |
| `Project_Charter_Oficial.docx` | Termo de Abertura formal com objetivos SMART, premissas, restrições e marcos |
| `Escopo_e_EAP_Oficial.docx` | Fronteiras conceituais, critérios de aceitação e dicionário analítico da EAP |
| `Cronograma_e_Caminho_Critico_CPM.docx` | Planejamento temporal de 62 dias, cálculo de folgas e sequência crítica |
| `Gestao_de_Custos_e_ROI_Oficial.docx` | Orçamento acadêmico (R$ 14,3k), estudo industrial (R$ 31,9k) e Payback de 8 meses |
| `Registro_de_Riscos_PMBOK_Oficial.docx` | Matriz de 7 riscos (R01 a R07) com causas-raiz e planos de contingência |
| `Gestao_Comunicacao_Stakeholders_RACI.docx` | Mapeamento de partes interessadas, matriz RACI e rituais de comunicação |
| `Planejamento_da_Qualidade_Oficial.docx` | Conformidade com ABNT NBR ISO/IEC 17025, VIM e metas de assertividade |
| `Gestao_de_Recursos_e_Equipas_Oficial.docx` | Dimensionamento da equipe (480 h técnicas) e regras do time (*Team Charter*) |
| `Gestao_de_Mudancas_e_Integracao_Oficial.docx` | Fluxo de controle de mudanças (CCB), formulário CR-01 e lições aprendidas |
