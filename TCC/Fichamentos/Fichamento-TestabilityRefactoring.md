# Testability Refactoring in Pull Requests: Patterns and Trends

REICH, Pavel; MAALEI, Walid. Testability refactoring in pull requests: Patterns and trends. In: 2023 IEEE/ACM 45th International Conference on Software Engineering (ICSE). IEEE, 2023. p. 1508-1519.

## 1. Fichamento de Conteúdo

O desenvolvimento de software moderno impõe um grande desafio na garantia de qualidade, com os desenvolvedores dedicando uma parcela significativa de seu tempo a testes, em especial testes de unidade. Contudo, sistemas não concebidos com a testabilidade em mente frequentemente exigem esforços adicionais de refatoração para que suas unidades de código se tornem mais observáveis e controláveis, permitindo um teste isolado e eficaz. Este artigo aborda a questão de como os desenvolvedores refatoram o código de produção para otimizar a testabilidade, identificando padrões de refatoração que facilitam a criação e aprimoramento de testes de unidade. A metodologia empregou uma análise mista, combinando mineração automática de milhares de *pull requests* (PRs) Java no GitHub com a análise manual detalhada de 724 PRs. Este método rigoroso visou identificar e caracterizar *padrões de refatoração de testabilidade*, classificando PRs que co-modificavam código de produção e de teste como "Test-Pairs PRs". Os resultados revelaram que as Test-Pairs PRs são mais intensivas em refatoração do que outras, e que cerca de 25% das PRs analisadas manualmente continham padrões de refatoração de testabilidade. Foram identificados dez *padrões recorrentes*, predominantemente voltados para a quebra de dependências, como a extração de métodos ou o alargamento do acesso a funcionalidades, visando facilitar o teste isolado.

## 2. Fichamento Bibliográfico

*   **Refatoração de Testabilidade:** Procedimentos compostos de refatoração realizados no código de produção com o propósito explícito de melhorar sua capacidade de ser testado, especialmente por testes de unidade. Isso envolve tornar o código mais observável e controlável, geralmente para quebrar dependências.
*   **Test-Pairs PRs:** *Pull requests* que incluem mudanças tanto no código de produção quanto no código de teste, indicando uma co-evolução intencional para melhorar a testabilidade da unidade de software.
*   **Refatorações Atômicas:** Ações de refatoração de granularidade fina, como "mudar tipo de variável", "extrair operação" ou "adicionar parâmetro", que podem ser detectadas automaticamente por ferramentas e que compõem os padrões de refatoração de testabilidade.
*   **Padrões de Refatoração de Testabilidade (Composite Refactoring Procedures):** Dez procedimentos de refatoração de alto nível, recorrentes e coerentes, identificados no estudo, que combinam refatorações atômicas para melhorar a testabilidade. Exemplos incluem "extrair método para *override*" ou "extrair classe para invocação".
*   **Quebra de Dependências:** O objetivo principal de muitos *padrões de refatoração de testabilidade*, que visam isolar uma classe sob teste de suas dependências para permitir o uso de objetos *mock* ou *stub* e facilitar o teste unitário.

## 3. Fichamento de Citações

*   "To create unit tests, it may be necessary to refactor the production code, e.g. by widening access to specific methods or by decomposing classes into smaller units that are easier to test independently."
*   "About 25% of all analyzed pull requests actually included testability refactoring patterns."
*   "If not designed with unit testing in mind, software systems might need extra refactoring effort to improve its observability and controllability, enabling a better testability."
*   "Our results indicate the pattern frequencies, in which pull requests they can be expected, and with what atomic refactorings they co-occur."
*   "Test-Pairs PRs are more refactoring intensive than other PRs."
*   "Clearly, the majority of the discovered patterns aim at breaking dependencies between the classes under test in order to test them in isolation."