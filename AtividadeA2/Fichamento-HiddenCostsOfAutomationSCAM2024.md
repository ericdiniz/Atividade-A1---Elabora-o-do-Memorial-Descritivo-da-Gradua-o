# The Hidden Costs of Automation: An Empirical Study on GitHub Actions Workflow Maintenance

VALENZUELA-TOLEDO, Pablo et al. The hidden costs of automation: An empirical study on github actions workflow maintenance. In: 2024 IEEE International Conference on Source Code Analysis and Manipulation (SCAM). IEEE, 2024. p. 213-223.

## 1. Fichamento de Conteúdo

A automação de tarefas de engenharia de software, especialmente através de práticas contínuas (*CI/CD*), é amplamente adotada para agilizar processos e reduzir falhas. Este artigo investiga os “custos ocultos” dessa automação, com foco na manutenção dos arquivos de *workflow* em *YAML* do *GitHub Actions*. O estudo empírico analisou 183 projetos maduros no GitHub, selecionados por critérios de atividade (≥ 8.151 *commits*), popularidade (≥ 28.691 estrelas), número de contribuidores (≥ 135) e uso de *GitHub Actions* em dez linguagens de programação. A metodologia consistiu na análise longitudinal do histórico de *commits* para medir volume de mudanças, taxa de evolução, acoplamento lógico com outros arquivos e propriedade dos *workflows*. Os resultados revelaram que esses arquivos mudam menos frequentemente que o código de produção ou de teste, mas possuem tamanho médio semelhante e exigem manutenção recorrente. As principais motivações de alteração foram correções de *bugs* e melhorias de *CI/CD*. Poucos desenvolvedores se especializam nos *workflows*, mas geralmente atuam também em produção e testes. Assim, o artigo evidencia que, embora a automação otimize fluxos de desenvolvimento, ela acarreta custos de manutenção que precisam ser planejados e apoiados por melhores práticas e ferramentas de suporte.

## 2. Fichamento Bibliográfico

* **GitHub Actions (GA):** Uma plataforma de orquestração integrada ao GitHub, que permite a automação de tarefas de engenharia de software como *build*, *test* e *deployment* através de arquivos de *workflow* YAML, sendo amplamente adotada para implementar Práticas Contínuas (CP).
* **Manutenção de Workflow:** O esforço humano requerido para corrigir defeitos, atualizar dependências e refatorar arquivos de *workflow* do GitHub Actions. O estudo enfatiza que essa manutenção representa uma carga de trabalho adicional e "custos ocultos da automação", apesar da premissa de que a automação simplificaria esses processos.
* **Acoplamento Lógico de Workflow:** A interdependência entre arquivos de *workflow* e outros arquivos do projeto (código de produção ou teste), medida pela frequência com que as mudanças ocorrem juntas no mesmo *commit*. A pesquisa indicou que o acoplamento é mínimo e fraco, embora ligeiramente maior com arquivos de produção do que com arquivos de teste.
* **Drivers de Manutenção de GA:** As razões subjacentes que impulsionam as modificações nos arquivos de *workflow* do GA. O estudo identificou as melhorias de CI/CD e as correções de *bugs* como os principais fatores, seguidos por atividades de gerenciamento e configuração, e esforços de teste e documentação.
* **Propriedade de Workflow:** A distribuição das responsabilidades de desenvolvimento e manutenção dos arquivos de *workflow* entre os membros da equipe. A análise revelou que poucos desenvolvedores se especializam em *workflows*, mas aqueles que o fazem frequentemente possuem conhecimento cross-funcional, atuando também em código de produção e de teste.

## 3. Fichamento de Citações

* "Although GA workflows are the primary means for automation, according to our experience and observations, human intervention is necessary to correct defects, update dependencies, or refactor existing workflow files."
* "This suggests that workflow files, which are also used to automate repetitive tasks in professional software production, may generate extra workload for developers."
* "Our findings largely confirm the results of previous studies on the maintenance of similar artifacts, while also revealing GA-specific insights such as bug fixing and CI/CD improvement being among the major drivers of GA maintenance."
* "On the one hand, as expected, we find that workflow files constitute a rather small proportion of a project’s total amount of files, and that they are changed less frequently than other kinds of source code files."
* "However, the average size of workflow files is comparable to those of production and test code files, and they are far from being stable in terms of evolution."
* "Practitioners should be aware that while automation through GA workflows helps to streamline the CI/CD process, it also incurs significant maintenance efforts expressed in workflow modifications."
