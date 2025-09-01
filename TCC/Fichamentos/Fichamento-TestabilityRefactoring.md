# Testability Refactoring in Pull Requests: Patterns and Trends

REICH, Pavel; MAALEI, Walid. Testability refactoring in pull requests: Patterns and trends. In: 2023 IEEE/ACM 45th International Conference on Software Engineering (ICSE). IEEE, 2023. p. 1508-1519.

## 1. Fichamento de Conteúdo

O artigo investiga como desenvolvedores realizam refatorações para melhorar a testabilidade de sistemas, especialmente no contexto de testes unitários. O estudo analisou 346.841 *pull requests (PRs)* em 621 projetos Java do GitHub, distinguindo entre PRs que co-modificam código de produção e de teste (chamadas *Test-Pairs PRs*) e PRs sem essa co-modificação. A metodologia seguiu três etapas: (i) análise automatizada com o *RefactoringMiner*, identificando 273.201 refatorações em 7.782 *Test-Pairs PRs* contra 114.427 em 4.839 *pull requests (PRs)* sem pares; (ii) amostragem incremental de 724 *pull requests (PRs)* para análise manual detalhada, apoiada em técnicas de *Grounded Theory*, *Thematic Analysis* e *Content Analysis*; (iii) validação cruzada por equipe de pesquisadores e pós-graduandos para reduzir vieses de classificação. Os resultados mostraram que *Test-Pairs *pull requests (PRs)** são significativamente mais refatoração-intensivos (média de 34,9 refatorações por PR, contra 23,6 em *pull requests (PRs)* comuns) e concentram mudanças maiores em linhas de código. Foram identificados 10 padrões recorrentes de refatoração para testabilidade, como *extract method for override*, *widen access for invocation* e *extract class for invocation*, sendo que aproximadamente 25% dos *pull requests (PRs)* analisados manualmente apresentaram ao menos um desses padrões. A maioria das práticas visa quebrar dependências e tornar o código mais observável e controlável, facilitando testes isolados. Assim, o estudo fornece evidências empíricas de que melhorar a testabilidade exige refatorações específicas e recorrentes, que podem servir como base para catálogos de boas práticas, *templates em IDEs* e diretrizes educacionais.

## 2. Fichamento Bibliográfico

* **Refatoração de Testabilidade:** Procedimentos compostos de refatoração realizados no código de produção com o propósito explícito de melhorar sua capacidade de ser testado, especialmente por testes de unidade. Isso envolve tornar o código mais observável e controlável, geralmente para quebrar dependências.
* **Test-Pairs PRs:** *Pull requests* que incluem mudanças tanto no código de produção quanto no código de teste, indicando uma co-evolução intencional para melhorar a testabilidade da unidade de software.
* **Refatorações Atômicas:** Ações de refatoração de granularidade fina, como "mudar tipo de variável", "extrair operação" ou "adicionar parâmetro", que podem ser detectadas automaticamente por ferramentas e que compõem os padrões de refatoração de testabilidade.
* **Padrões de Refatoração de Testabilidade (Composite Refactoring Procedures):** Dez procedimentos de refatoração de alto nível, recorrentes e coerentes, identificados no estudo, que combinam refatorações atômicas para melhorar a testabilidade. Exemplos incluem "extrair método para *override*" ou "extrair classe para invocação".
* **Quebra de Dependências:** O objetivo principal de muitos *padrões de refatoração de testabilidade*, que visam isolar uma classe sob teste de suas dependências para permitir o uso de objetos *mock* ou *stub* e facilitar o teste unitário.

## 3. Fichamento de Citações

* "To create unit tests, it may be necessary to refactor the production code, e.g. by widening access to specific methods or by decomposing classes into smaller units that are easier to test independently."
* "About 25% of all analyzed pull requests actually included testability refactoring patterns."
* "If not designed with unit testing in mind, software systems might need extra refactoring effort to improve its observability and controllability, enabling a better testability."
* "Our results indicate the pattern frequencies, in which pull requests they can be expected, and with what atomic refactorings they co-occur."
* "Test-Pairs PRs are more refactoring intensive than other PRs."
* "Clearly, the majority of the discovered patterns aim at breaking dependencies between the classes under test in order to test them in isolation"
