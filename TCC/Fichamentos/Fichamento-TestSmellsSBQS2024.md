# A Multimethod Study of Test Smells: Cataloging, Removal, and New Types

SOARES, Elvys; RIBEIRO, Márcio; SANTOS, André. A Multimethod Study of Test Smells: Cataloging Removal and New Types. In: Proceedings of the XXIII Brazilian Symposium on Software Quality. 2024. p. 676-686.

## 1. Fichamento de Conteúdo

O trabalho investiga lacunas persistentes na área de *test smells*, que são sintomas no código de teste indicando potenciais problemas de design ou implementação. Apesar do conceito ser conhecido desde 2001, faltava um catálogo centralizado e uma compreensão aprofundada de como recursos modernos de *frameworks* de teste poderiam apoiar a refatoração e prevenção desses problemas, além da quase ausência de estudos sobre *smells* em testes manuais. A pesquisa adotou uma metodologia multimétodo: (i) uma Revisão Multivocal da Literatura (MLR) que analisou 127 estudos primários e consolidou 480 *test smells* distintos; (ii) um estudo empírico em 77 projetos *open-source* para avaliar o uso de novos recursos do JUnit 5; (iii) transformações propostas para 13 *smells* com base em 7 funcionalidades do JUnit 5, validadas por meio de *surveys* com 212 desenvolvedores de 39 países e *pull requests* aceitos em repositórios OSS (94% de aceitação); e (iv) um estudo exploratório de suítes de testes manuais, identificando oito novos *smells* de linguagem natural e validando uma ferramenta de detecção automática baseada em NLP, que alcançou precisão de 92%, *recall* de 95% e *f-measure* de 93,5%. Os resultados oferecem três grandes contribuições: um catálogo público e unificado de *test smells*, evidências de que novos recursos de *frameworks* ajudam a prevenir e remover problemas, e a expansão da análise de *smells* para testes manuais. Essas contribuições fortalecem tanto a prática industrial quanto a pesquisa acadêmica em qualidade de software.


### 2. Fichamento Bibliográfico

* **Test Smells**: Sintomas que aparecem no código de teste, sinalizando possíveis falhas de design ou implementação, semelhantes aos *code smells* no código de produção (p. 7, 8, 29). Sua presença em suítes de testes automatizados pode resultar em comportamentos erráticos, como testes instáveis ou resultados falsos.
* **Revisão de Literatura Multivocal (MLR)**: Uma abordagem de revisão sistemática que engloba tanto a literatura formal (artigos científicos, periódicos) quanto a literatura cinzenta (teses, blogs, relatórios técnicos), proporcionando uma visão mais completa do estado da arte e da prática em um determinado tópico (p. 15, 36, 61, 63).
* **Recursos do JUnit 5**: Novas funcionalidades introduzidas no *framework* de teste JUnit 5, como *Grouped Assertions*, *Execution Condition API*, *Repeated Test* e *ParameterizedTest*, que podem ser utilizadas para refatorar *test smells* e otimizar a escrita de testes (p. 7, 8, 51).
* **Natural Language Test Smells**: Problemas de design ou qualidade presentes em descrições de testes manuais, que são formuladas em linguagem natural, e que podem comprometer a clareza, a execução e a manutenção dos testes (p. 17, 34, 84). O estudo propõe 8 novos tipos específicos (p. 7, 8, 40).
* **Processamento de Linguagem Natural (NLP)**: Uma tecnologia de inteligência artificial utilizada para analisar e compreender o texto em linguagem humana. No contexto da tese, é aplicada para a detecção automatizada de *test smells* em descrições de testes manuais, baseando-se em análises sintáticas e morfológicas (p. 16, 41, 94).
* **Catálogo de Test Smells**: Um repositório *online* e público que reúne, organiza e mantém informações sobre os *test smells* identificados na literatura, incluindo suas definições, nomes alternativos e referências, servindo como um ponto de consulta centralizado para a comunidade (p. 7, 8, 37, 93).

### 3. Fichamento de Citações

* "Test smells are symptoms in the test code that indicate possible design or implementation problems."
* "Although test smells have been the subject of much gray and academic literature since their proposal in 2001, many questions regarding their ad-herence in the industry are yet to be clarified: concerning test smells — proposed by numerous studies and gray literature — **no publicly available catalog aggregates them**"
* "The results present: (i) a catalog that unifies 127 primary studies and 480 distinct test smells in a previously unseen effort"
* "The results present: (ii) the confirmation that **new test framework features can refactor and prevent test smells**"
* "The results present: (iii) the proposition of a catalog containing 8 new test smells specific to manual test suites, their identification strategies based on natural language processing, and their frequency in important government, industry and open-source systems."
* "We develop a NLP-based tool that reaches a precision of 92%, recall of 95%, and f-measure of 93.5%, indicating a suitable detection level for our proposals."
