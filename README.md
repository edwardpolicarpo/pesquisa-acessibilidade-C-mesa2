# Investigação de Acessibilidade Digital: Dimensão C (Legislação)

*Escola de Tecnologia — Instituto J&F (DAD 2026)*

---

## Sobre a pesquisa

Esta investigação analisa o **arcabouço jurídico da acessibilidade digital**, com foco na seguinte questão:

> **Quais leis obrigam a acessibilidade digital e quais são as consequências para empresas e desenvolvedores?**

O objetivo é compreender não apenas a existência das normas, mas também seus impactos práticos no desenvolvimento de sistemas e interfaces digitais.

---

## Principais achados

* **Obrigatoriedade legal no Brasil**
  A **Lei Brasileira de Inclusão (Lei nº 13.146/2015)**, especialmente em seu Art. 63, estabelece que **sites de empresas com atuação no Brasil devem ser acessíveis a pessoas com deficiência**, prevendo sanções em caso de descumprimento.

* **Riscos jurídicos no cenário internacional**
  Nos Estados Unidos, a **Americans with Disabilities Act (ADA)** tem sido aplicada a ambientes digitais, resultando em um crescimento expressivo de ações judiciais relacionadas à falta de acessibilidade, especialmente a partir de 2023.

* **Padronização no setor público brasileiro**
  O **Modelo de Acessibilidade em Governo Eletrônico (e-MAG)** define diretrizes técnicas obrigatórias para portais e serviços digitais do governo federal.

* **Baixa conformidade global**
  Segundo o relatório **WebAIM Million (2024)**, aproximadamente **96,3% das páginas mais acessadas do mundo apresentam falhas de acessibilidade**, evidenciando um cenário de alto risco jurídico e técnico.

---

## Linha do tempo da legislação

|    Ano   | Marco Legal           | Descrição e Impacto                                                                                   |
| :------: | :-------------------- | :---------------------------------------------------------------------------------------------------- |
| **1990** | ADA (EUA)             | Lei de direitos civis que fundamenta a acessibilidade, atualmente aplicada também ao ambiente digital |
| **2014** | e-MAG (Brasil)        | Estabelece diretrizes técnicas obrigatórias para sistemas governamentais                              |
| **2015** | LBI (Brasil)          | Principal marco legal brasileiro; torna a acessibilidade digital obrigatória no setor privado         |
| **2018** | WCAG 2.1              | Diretrizes internacionais que orientam a implementação técnica da acessibilidade                      |
| **2023** | Aumento de litigância | Crescimento significativo de ações judiciais relacionadas à acessibilidade digital                    |

---

## Impactos para desenvolvedores

A conformidade com a legislação depende diretamente de práticas técnicas adotadas durante o desenvolvimento. Destacam-se três medidas essenciais:

### 1. Documentação de conformidade

A utilização de ferramentas como **Lighthouse** e **axe-core** deve ser incorporada ao fluxo de desenvolvimento.
Recomenda-se armazenar evidências (relatórios ou capturas) a cada deploy, garantindo rastreabilidade e comprovação de boas práticas.

---

### 2. Uso adequado de semântica HTML

A estruturação correta do HTML é fundamental para acessibilidade.

Boas práticas incluem:

* Utilização de elementos semânticos (`<button>`, `<nav>`, `<main>`)
* Aplicação adequada de atributos ARIA quando necessário

Falhas nesse aspecto estão entre as principais causas de não conformidade.

---

### 3. Gerenciamento de foco e navegação

Interfaces devem ser totalmente navegáveis por teclado.

Exemplo de implementação:

```javascript
const modal = document.querySelector('#meuModal');
modal.focus();
```

A ausência de controle de foco compromete o uso por tecnologias assistivas, configurando não conformidade com a legislação.

---

## Considerações finais

A acessibilidade digital deixou de ser apenas uma recomendação técnica e passou a ser uma **exigência legal**.

O não cumprimento pode resultar em:

* Sanções administrativas
* Processos judiciais
* Impactos reputacionais

Dessa forma, a adoção de práticas acessíveis deve ser tratada como parte integrante do desenvolvimento de software.

---

## Referências

1. BRASIL. Lei nº 13.146/2015 (Lei Brasileira de Inclusão). Disponível em: https://www.planalto.gov.br/ccivil_03/_ato2015-2018/2015/lei/l13146.htm
2. GOVERNO FEDERAL. Modelo de Acessibilidade em Governo Eletrônico (e-MAG). Disponível em: https://emag.governoeletronico.gov.br/
3. U.S. Department of Justice. Guidance on Web Accessibility and the ADA. Disponível em: https://www.ada.gov/resources/web-guidance/
4. W3C Brasil. WCAG 2.1 — Tradução Autorizada. Disponível em: https://www.w3.org/Translations/WCAG21-pt-BR/
5. WebAIM. The WebAIM Million: 2024 Report. Disponível em: https://webaim.org/projects/million/

---
