Análise das Evidências {#sec:analise_evidencias_srl}
----------------------

Nessa seção, são apresentados os resultados para cada questão de
pesquisa. Na são apresentadas evidências quanto aos desafios relatados
na adoção de práticas contínuas.Na subseção são apresentadas as
evidências quanto as boas práticas para implementar com êxito práticas
contínuas. Na são descritas as ferramentas que são utilizadas para
projetar e implementar pipelines de implantação. Todas as evidências são
devidamente referenciadas pelos 54 estudos, e os números das referências
são precedidos por EP (Estudo Primário), como forma de deixar claras as
referências da revisão sistemática. Como anteriormente citado, as
informações quanto aos EP estão disponíveis no .

### Q1. Quais desafios foram relatados para a adoção de práticas contínuas? {#subsec:srl_rq1_desafios}

Esta questão buscou investigar os principais desafios em relação a
adoção de um pipeline de implantação. A partir dos 54 estudos primários
analisados, 32 desafios foram identificados pela pesquisa. Os desafios
foram agrupados em 9 categorias, sendo elas: Humano e Organizacional,
Processo, Ferramentas, Design de Compilação, Integração, Arquitetura da
Aplicação, Teste e Qualidade, Entrega, Infraestrutura e Monitoramento.
As evidências quanto a essas questões são descritas abaixo e sumarizadas
na .

### Humano e Organizacional {#humano-e-organizacional .unnumbered}

Esta seção listará os desafios relacionados aos aspectos humanos e a
estrutura organizacional de uma empresa, e, como podem afetar a
implementação do . Os problemas mais relatados neste tema foram questões
culturais, falta de comunicação e curva de aprendizado íngreme, falta de
habilidades e desafios organizacionais.

#### D1. Questões Culturais {#d1.-questões-culturais .unnumbered}

As questões culturais são vistas como um grande desafio na adoção de
práticas de entrega contínua (EP\_26), pois para que sejam adotadas tais
práticas se faz necessário mudanças profundas na mentalidade. Essa
mudança pode ser tornar um desafio maior se a cultura organizacional for
arraigada (EP\_52). Riungu-Kalliosaari et al. (EP\_52) citam como
exemplo o caso dos desenvolvedores que precisam assumir tarefas com as
quais não estão acostumados e podem ter reservas em aceitar novas
responsabilidades.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_19** – *“Cultural issues. The largest cultural issue is
    created by the customer’s culture of project management.”*

-   **EP\_26** – *“The principles and practices of continuous delivery
    can be implemented in all kinds of environments, from mainframes to
    firmware to those that are highly regulated, but it’s certainly not
    easy.[...] Typically, the biggest obstacles to this transformation
    are organizational culture and architecture.”*

-   **EP\_52** – *“DevOps adoption also highlights cultural matters.
    Profound changes to the cultural mindset are required and the
    deep-seated company culture can be a challenge.[...] The cultural
    aspects are significant, as has been previously stated [7,13]. The
    size of the company or having company-wide support for the change
    might matter. Smaller companies are in a better position to react
    faster to changes.”*

#### D2. Cliente desmotivado {#d2.-cliente-desmotivado .unnumbered}

Para se adotar práticas de contínuas o cliente precisa estar envolvido
ativamente na implantação contínua e automática. Shahin et al. (EP\_14)
dizem que embora as empresas pudessem fornecer entregas com a maior
frequência possível as organizações de seus clientes, as culturas e
políticas estabelecidas nelas, não suportavam a transição completa para
a prática de , e portanto, as empresas tiveram que seguir intervalos de
tempo predefinidos para lançar o software.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“We found that not all customers are mature enough to
    accept a continuous release.”*

#### D3. Curva de aprendizado íngreme {#d3.-curva-de-aprendizado-íngreme .unnumbered}

Um pipeline de implantação bem estabelecido ajuda os novos membros a se
familiarizarem rapidamente, no entanto, eventualmente, eles precisam
aprender a atualizar o pipeline de implantação (EP\_28). No caso de
mudanças no pipeline, Zhang et al. (EP\_36) afirmam que caso os
desenvolvedores encontrem uma maior complexidade, maior latência e menor
confiabilidade em fluxos de trabalho de CD anteriores, essas barreiras
farão com que eles mudem para novos fluxos de trabalho de CD.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_28** – *“High skills and knowledge demands. DevOps practices
    require that, in the least, the team as a whole has all necessary
    skills and knowledge to develop, integrate, test and deploy, which
    includes provisioning and upkeep target environments and
    infrastructure.”*

-   **EP\_36** – *“Steep learning curve. Complex processes and
    unfamiliar configurations make some developers abandon their old
    workflow. Like R76 told, their old workflow was “hard to learn,
    configure, or plain inefficient”.”*

#### D4. Dependências da equipe {#d4.-dependências-da-equipe .unnumbered}

A arquitetura de um aplicativo determina, em grande parte, a estrutura
da equipe de desenvolvimento que trabalha nesse aplicativo (E\_21).
Shahin, Babar e Zhu (E\_21) relatam ainda em seu estudo, que este
desafio foi observado em equipes grandes que trabalhavam em uma base de
código monolítica, no qual, para a implementação da aplicação, essas
grandes equipes se dividiam em equipes menores.

As várias equipes trabalhando simultaneamente, geram uma dependência
entre elas. Nessa situação pode haver equipes que tenham o controle do
processo de implantação, que dependerão da liberação de outras equipes.
A modificação desenvolvida por uma equipe pode causar falha de *build*.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_21** – *“One of the challenges reported by the participants
    was that the dependent teams working on monolithic large-codebase
    were not successful in adopting and implement CD practice.”*

#### D5. Falsa sensação de confiança {#d5.-falsa-sensação-de-confiança .unnumbered}

Outro desafio relatado é a falsa sensação de confiança, que trata-se de
uma situação em que os desenvolvedores confiam cegamente nos testes.
Essa falsa sensação pode levar um revisor de código a mesclar sem uma
revisão completa.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_33** – *“Another recurring problem is the false sense of
    confidence (25 occurrences). As opposed to the confidence benefit,
    respondents described the false sense of confidence as a situation
    where developers blindly trust the tests. One respondent synthesized
    this problem as follows”*

#### D6. Falta de comunicação {#d6.-falta-de-comunicação .unnumbered}

A melhora da comunicação é considerado um dos benefícios de práticas
continuas, no entanto, a falta dela dificulta a solução da tarefa
ocasionando uma quebra no *build* (EP\_33). Mårtensson et al. (EP\_07)
afirmam que a comunicação entre as equipes pode faltar, e
Riungu-Kalliosaari et al. (EP\_52) diz que se ela ocorrer apenas por
meio de sistemas eletrônicos, causará atrasos nos tempos de reação aos
problemas.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_07** – *“One workshop participant from Company C described the
    presentation as “representative” and added “there are a lot of
    problems with communication between teams”.”*

-   **EP\_33** – *“Still, we found six respondents that claimed that the
    lack of communication hindered the solution of a task, leading to
    build breakage.”*

-   **EP\_52** – *“The respondents raised challenges related to
    communication patterns, organization cultures which are not
    malleable, different constraints stemming from the domain and
    environments, and the obscurity of the meaning of DevOps”*

#### D7. Falta de conhecimento de domínio {#d7.-falta-de-conhecimento-de-domínio .unnumbered}

A falta de conhecimento do domínio, pode impedir as contribuições de
colaboradores novos, que sem orientação ou documentação adequada, não
sabem como o projeto é organizado ou como começar a contribuir (EP\_33).
Pinto et al. (EP\_33) afirmam que essa dificuldade é particularmente
relevante para projetos de código aberto projetos de código aberto.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_33** – *“Moreover, lack of domain knowledge, mentioned by 18
    respondents, might hinder contributions from external contributors
    (eg, “lack of familiarity with a specific project”).”*

#### D8. Falta de habilidades {#d8.-falta-de-habilidades .unnumbered}

A equipe precisa ter todas as habilidades e conhecimentos necessários
para desenvolver, integrar, testar e implantar, incluindo o
provisionamento e manutenção de ambientes e infraestrutura de destino.
Um pipeline de implantação bem estabelecido ajuda os novos membros a se
familiarizarem rapidamente, pois esses, precisaram aprender sobre o
pipeline (EP\_28).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_19** – *“Skills. The team needs to have a sufficient knowledge
    of what can be done and how to do it to be able to aim for higher CD
    maturity. Furthermore there is a need to have access to training to
    improve available skill set.”*

-   **EP\_28** – *“DevOps practices require that, in the least, the team
    as a whole has all necessary skills and knowledge to develop,
    integrate, test and deploy, which includes provisioning and upkeep
    target environments and infrastructure.”*

#### D9. Desafios organizacionais {#d9.-desafios-organizacionais .unnumbered}

As estruturas organizacionais podem ser desafios significativos na
implementação da (EP\_42). Uma organização distribuída pode ocasionar
problemas de comunicação, dificultando a correção de falhas de
compilação (EP\_25). Chen (EP\_42) declara que deve-se mudar o estrutura
organizacional existente para criar implementações de sucesso.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_25** – *“Distributed Organization. The case organization was
    distributed to several sites and countries. The participants thought
    that the communication was not working between the sites, especially
    when there were cultural differences. The communication problems
    were shown during the CD adoption by surprising breaking changes.
    These included API changes, version changes of libraries or changes
    in installation scripts. The breaking changes caused failing
    builds.”*

-   **EP\_42** – *“I mentioned organizational challenges in my earlier
    paper (Chen, 2015a). However, apart from the points discussed in
    Chen (2015a), I recently noticed another area in which
    evidence-based results are important. Organizational structures can
    be a significant barrier when implementing CD (Chen, 2015a).”*

### Processo {#processo .unnumbered}

Esta seção listará os desafios diretamente ou indiretamente relacionados
ao processo de desenvolvimento da equipe que deseja implementar práticas
contínuas. Mesmo que essas práticas não estejam diretamente relacionadas
a um processo de desenvolvimento específico, foram encontrados
diferentes aspectos do processo que podem tornar mais difícil a adoção
das práticas contínuas com sucesso.

#### D10. Ambientes heterogêneos {#d10.-ambientes-heterogêneos .unnumbered}

Em ambientes heterogêneos há uma dificuldade na replicação dos serviços
em produção para o ambiente para verificação e teste, pois tais serviços
podem ser complexos o suficiente para dificultar tal replicação,
tornando o teste automatizado se torna menos confiável.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_21** – *“Our analysis of the data revealed that it was
    challenging for a couple of practitioners to design applications for
    different operations environments, in which they may have had
    difficulty to make consistency in a set of heterogeneous operations
    environments in order to seamlessly transfer and deploy the
    application in all production environments.”*

-   **EP\_52** – *“As a consequence, automated testing becomes less
    trustworthy meaning that heterogeneous environments provide a
    challenge for successful DevOps adoption.”*

#### D11. Múltiplos Ambientes {#d11.-múltiplos-ambientes .unnumbered}

Em um determinado aplicativo, pode haver a necessidade de se tem que ter
vários ambientes por inúmeras razões, como exemplo de ambiente tem-se,
local, desenvolvimento, *staging* e produção. Nesse caso, ter vários
ambientes também pode ser um problema, pois se a compilação falhar,
poderá ser difícil depurá-la, especialmente se o problema não ocorrer no
ambiente local.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_33** – *“Interestingly, one respondent drew attention to the
    fact that the benefit multiple environments can also be a problem,
    [...]”*

### Ferramentas {#ferramentas .unnumbered}

Nesta seção, será abordado os desafios associados às ferramentas usadas
durante a implementação da integração e entrega contínua.

#### D12. Ferramentas em constante mudança {#d12.-ferramentas-em-constante-mudança .unnumbered}

Alguns profissionais acabam obtendo muito conhecimento em relação a um
determinado tipo de ambiente e provavelmente projetando sistemas com
especificidades para esse determinado tipo de ambiente. Se o ambiente
mudar as decisões de design específicas não funcionaram. A influência de
ferramentas em constante mudança no design de arquitetura para permitir
a prática do CD acaba se tornando um desafio (EP\_21).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_21** – *“Another challenge reported at architectural level was
    the influence of ever-changing environments and tools on
    architecture design to enable CD practice.”*

#### D13. Falta de suporte de ferramenta {#d13.-falta-de-suporte-de-ferramenta .unnumbered}

Quando uma equipe o planjamento de adoção de um pipeline / deve-se tomar
muito cuidado com a escolha de ferramentas, pois uma determinada tarefa
pode não atender ao que se esperava, podendo ocasionar um retrabalho
para migrar para outra ferramenta que atenda melhor. Debroy, Miller e
Brimble (EP\_35) em seu estudo por ainda não terem a licença do Google
Cloud basearam-se na integração do Visual Studio Team Services e Azure,
no entanto, essa escolha de ferramenta impossibilitou-os de registrar os
container no com Google Container Registry, causando um atraso na adoção
do pipeline /.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_35** – *“At this point, it looked like due to lack of tool
    support – we were either going to have to give up Google Cloud as an
    option or create entirely new CI/CD pipelines to support it.”*

### Design de Compilação {#design-de-compilação .unnumbered}

Está seção abordará os desafios causados por decisões de design de
compilação.

#### D14. Longos tempos de espera para *builds* {#d14.-longos-tempos-de-espera-para-builds .unnumbered}

Uma compilação demorada reflete no modo de trabalho da equipe de
desenvolvimento, afetando a eficiência, fazendo com que alguns
desenvolvedores mudem seus fluxos de trabalho. Debroy, Miller e Brimble
(EP\_35) relatam o problema que tiveram em aplicação monolitica que
estava migrando para arquitetura microsserviços, na qual, a construção
dos microsserviços era realizada pelo pipeline /. Como haviam muitos
microsserviços distribuidos entre várias equipes os *builds* entraram
numa fila, gerando atrasos e muito tempo perdido.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_35** – *“Long Wait Times for Builds/Releases: At least one of
    the problems becomes evident when we directly apply the existing
    CI/CD setup as-is to support the desired goals[...]”*

-   **EP\_36** – *“Overly long build times. As we found earlier when
    asking about CD needs, build speed affects the developers’ work
    efficiency.”*

### Integração {#integração .unnumbered}

Esta seção listará os desafios que surgem quando o código é integrado à
ramificação principal do controle de versão.

#### D15. *Branches* longas {#d15.-branches-longas .unnumbered}

Trabalhar em ramificações ou *branches* longas vai de encontro com a
filosofia da integração contínua, pois a integração da nova
funcionalidade é adiada, ocasionando grandes problema de integração.
M<span>å</span>rtensso, Hammarstr<span>ö</span>me e Bosch (EP\_03)
relataram esse desafio a prática GitFlow, informando que os
desenvolvedores preocupam-se em integra constantemente na *branch* de
desenvolvimento do que na principal, fazendo com que as entregas na
*branch* principal não possuam valor.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_03** – *“The third factor “no evident value in delivering
    often to the mainline” (shown in Fig. 7) include comments from only
    five interviewees. However, we believe that the interview responses
    on previous questions, describing a way of working with long-lived
    branches and delivering with a low frequency to the mainline
    supports “no evident value” as an important factor.”*

-   **EP\_07** – *“The product’s architecture: During the interviews, we
    identified problems related to teams working on a branch too long,
    and then having huge problems when they try to integrate (described
    in described Section IV-B).”*

#### D16. Falhas de *Build* {#d16.-falhas-de-build .unnumbered}

As falhas de construção não necessariamente são um problema para a
prática de , no entanto, se tornarão problemáticas se forem comuns e não
forem corrigidas imediatamente (EP\_25). Pinto et al. (EP\_33) relataram
diversas causas para as falhas de construção, como por exemplo, testes
inadequados, mudanças de versão da linguagem, complexidade da base de
código, entre outros.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_25** – *“Failing builds: CD pipeline builds were often failing
    and not fixed immediately afterwards.”*

-   **EP\_33** – *“We found several technical reasons that might explain
    build breakage. Among the most common ones, there is inadequate
    testing[...]”*

#### D17. Múltiplos *Branches* {#d17.-múltiplos-branches .unnumbered}

O uso de múltiplos *branches* no controle de versão atrasa a integração
do novo código a ramificação principal, fazendo com que o
desenvolvimento se torne complexo, pois equipes diferentes trabalhavam
em ramos diferentes, gerando uma dificuldade na comunicação, além de que
as correções de *bugs* e até mesmo novos recursos às vezes tinham que
ser aplicados a várias ramificações, exigindo um esforço adicional
(EP\_25).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_05** – *“Foi identificado que alguns sistemas possuíam muitas
    ramificações, o que dificultava a junção do código (merge) dos
    diversos ramos de desenvolvimento do sistema, quando era necessário
    gerar uma nova versão para ser testada.”*

-   **EP\_25** – *“In addition, working with multiple branches was
    described to cause complexity during development.”*

### Arquitetura da Aplicação {#arquitetura-da-aplicação .unnumbered}

Nesta seção, será examinado os desafios relacionados à arquitetura do
aplicação. Alguns tipos de arquitetura podem tornar muito difícil a
implementação do .

#### D18. Arquitetura Altamente Acoplada {#d18.-arquitetura-altamente-acoplada .unnumbered}

A arquitetura altamente acoplada é um desafio que está relacionado com a
adoção de práticas de implantação contínua em aplicativos monolíticos
pelas organizações. Esse tipo de sistema possui muitas dependências
multifuncionais, nas quais cada dependência precisa ser gerenciada no
pipeline de para implantação de software, portanto se um componente
precisar ser implantado no ambiente de produção, espera-se que todas as
dependências sejam implantadas juntamente com ele (EP\_21).

Os aplicativos podem ser monolíticos do ponto de vista do banco de
dados, ou seja, a aplicação ter uma arquitetura de microsserviços e usar
um único banco de dados ao invés de cada serviço possuir seu próprio
banco. Nesse caso, o banco de dados pode criar gargalos operacionais e
gradualmente se torna uma unidade não implantável, pois a alteração de
qualquer funcionalidade no aplicativo pode ocasionar mudanças no esquema
de banco de dados também (EP\_21).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_21** – *“Our analysis has revealed that highly coupled
    architecture presents the biggest challenge when organizations are
    going to move to continuous deployment practice.”*

-   **EP\_25** – *“Unsuitable Architecture. The participants reported
    that the product architecture did not support the adoption of
    CD.[...] Other than that, the architecture required the whole
    product to be released as a whole.”*

-   **EP\_29** – *“Dependency (Tightly Coupled): As the size and
    complexity of a monolith grows, the dependencies across the system
    will be so strong that it will become difficult to change different
    parts of the monolithic system independently.”*

#### D19. Dependências {#d19.-dependências .unnumbered}

O gerenciamento de dependências e o controle de versão são atividades
principais dos sistemas de *build*, no entanto, às vezes os
desenvolvedores não atualizam as dependências, logo o servidor de
detecta erros que não aconteceriam localmente. Pinto *et al.l* (EP\_33)
dizem que a maioria dos erros de compilação se deve à falta de
dependências.

A dependência de aplicações com outros sistemas podem inibir as
organizações a mudar de entrega contínua para implantação contínua, pois
isso significa que elas precisariam garantir que não haja nenhum
problema de integração ao implantar um aplicativo para produção
(EP\_14).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“Our study has found that albeit an application might
    be at deployable state, dependencies between that application and
    other systems may have inhibited some of the participants’
    organizations to transition from CDE to CD.”*

-   **EP\_29** – *“External dependencies with other applications were
    another roadblock to frequent deployment [...]”*

-   **EP\_33** – *“It is important to note that dependency management
    and version changes are two key activities of build systems.
    Therefore, developers that may face technical problems with the
    usage of build systems may also face those with CI systems.”*

#### D20. Restrições de Domínio {#d20.-restrições-de-domínio .unnumbered}

As restrições de domínio fazem com surjam muitos desafios na
aplicabilidade do , podendo alterar a frequência de liberação de
software (mudanças) para produção. Embora a prática de entrega contínua
seja facilmente aplicada a aplicativos baseados na web, ela pode se
tornar difícil se aplicada a outros domínios, como sistemas embarcados e
sistemas financeiros (EP\_14 apud Skelton e O’Dell, 2016).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“Many challenges in the applicability of CD arise due
    to domain constraints.”*

### Teste {#teste .unnumbered}

Nesta seção, serão discutidos os desafios relacionados aos testes de
software na adoção de um pipeline /. A parte central desse pipeline
envolve os testes automatizados, sendo o conjunto de testes executado
toda vez que há uma mudança na base de código, para validar que a
mudança pode ir para a produção.

#### D21. Falta de Estratégia de Teste {#d21.-falta-de-estratégia-de-teste .unnumbered}

A estratégia de teste defini os estágios e os tipos de teste que devem
ser usados e quando usá-los. A falta dessa estratégia faz com que sejam
produzidos testes redundantes e funcionalidades sejam testadas em nível
errado, gerando lentidão na execução pipeline (EP\_25).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_25** – *“The lack of a testing strategy had caused duplicate
    testing in the CD pipeline and the pipeline was considered slow
    because of that.”*

#### D22. Falta de Testes {#d22.-falta-de-testes .unnumbered}

Os testes automatizados garantem que o código produzido não irá
introduzir nenhum defeito ao sistema, além de aumentar a confiança da
equipe no produto de software. A falta de testes torna-se um desafio,
devido a que a execução de testes automatizados é uma das práticas
chaves para que a equipe possa colher os benefícios do .

Há diversos fatores que influenciam a falta de testes em um projeto.
Pinto et al. (EP\_33), em seu estudo, elenca a falta de cultura de
testes como um motivo social associado à quebra de construção, devido ao
fato de que os desenvolvedores não executam os testes e não constroem em
suas máquinas antes de enviarem as mudanças, delegando a execução dos
testes somente para o servidor . Já Laukkanen et al. (EP\_32 apud
Paternoster et al., 2014; Giardino et al., 2016) elencou a falta de
testes como uma das características da engenharia de lançamento das
*startups*, devido a falta de recusos.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_17** – *“Microservices introduces testing challenges, which
    mainly arise from changes that impact interactions among services.”*

-   **EP\_33** – *“In our study, we perceived that there is a lack of
    testing culture, which might motivate educators to place additional
    care in providing testing courses.”*

#### D23. Baixa Cobertura de Teste {#d23.-baixa-cobertura-de-teste .unnumbered}

O baixo nível de cobertura de testes reduz a confiança das organizações
na possibilidade de suas aplicações estarem prontas para serem
implantadas em produção (EP\_14, EP\_25). Essa baixa cobertura se torna
um desafio às práticas , pois ao prática-las deve-se estar confiante
para lançar o produto após a execução dos testes.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“Lack of sufficient automated test coverage was also
    deemed as a bottleneck to transition from CDE to CD [...].”*

-   **EP\_25** – *“The identified direct signs of a dysfunctional CD
    practice were failing builds, flaky tests, low test coverage and
    slow feedback. ”*

#### D24. Falta de Teste de Aceitação Automatizado {#d24.-falta-de-teste-de-aceitação-automatizado .unnumbered}

Os testes de aceitação tornam a construção do conjunto de teste mais
complexo e exigindo mais esforço para configurar e gerenciar testes
automatizados. Shahin et al. (EP\_14) relatou a preocupação que os
desenvolvedores tem sobre os benefícios potenciais de automatizar o
teste de aceitação em comparação com suas complexidades e custos
associados, elencando esta preocupação como um dos principais motivos
pelos quais esse tipo de teste não foram totalmente automatizados.

preocupações

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“The interviewees disclosed that they considerably
    succeeded in automating unit and integration tests, but automating
    the tests occurring at the end of development process such as (user)
    acceptance test and performance test has remained a challenge and
    requires heavy workloads and time.”*

#### D25. Testes Instáveis {#d25.-testes-instáveis .unnumbered}

*Flaky test* ou testes instáveis são testes que podem falhar
aleatoriamente na mesma configuração ou mesmo quando não há problemas na
alteração do código, por este motivo torna-ser difícil de reproduzir a
falha, dificultando a confiança nos resultados do *build* e aumentando o
esforço de manutenção da construção.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_25** – *“Some of the tests used in the CD pipeline were flaky
    and could fail randomly even if a software change did not have any
    problems in it. This makes it difficult to trust the build results
    and increases the build maintenance effort.”*

-   **EP\_33** – *“Moreover, seven respondents reported that flaky tests
    may affect only few jobs. A flaky test is a test that could fail or
    pass for the same configuration and, therefore, can create several
    problems since it can be hard to reproduce. ”*

#### D26. Testes de Longa Duração {#d26.-testes-de-longa-duração .unnumbered}

O feedback rápido é um dos benefícios da integração contínua, portanto
possuir testes de longa duração acarretará em um atraso do feedback dos
desenvolvedores, consequentemente, levará a um aumento do tempo do ciclo
de entrega.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“Long running tests not only increased the cycle time
    (i.e., the time required to get code from code repository into
    production) in a CDP, but also have hindered developers to getting
    real-time feedback.”*

#### D27. Teste Inadequado {#d27.-teste-inadequado .unnumbered}

A construção de testes inadequados é um das motivos mais comuns de uma
falha de construção, devido a falta de uma cultura de teste, o que leva
os desenvolvedores a pular ou escrever testes ruins e/ou ingênuos
(EP\_33).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_33** – *“Inadequate testing and time pressure are the most
    common technical and social reasons related to build breakage.”*

### Entrega {#entrega .unnumbered}

Esta seção listará os desafios relacionados a entrega e implantação de
software. Os problemas relacionados a entrega foram relatados em três
artigos, sendo eles, a falta de um mecanismo de reversão (EP\_14) e a
demora do processo de entrega (EP\_03, EP\_35).

#### D28. Falta de Mecanismo de Reversão {#d28.-falta-de-mecanismo-de-reversão .unnumbered}

A falta de um mecanismo de reversão eficiente força as empresas a
reduzir a frequência de lançamento de versões em produção, além de gerar
risco de entregar código com erros a seus clientes (EP\_14).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“ Lack of efficient and automated rollback mechanism
    to quickly recover issues in deployment process may put software
    organizations at risk of delivering buggy code to their customers.
    ”*

#### D29. Processo de Entrega Demorado {#d29.-processo-de-entrega-demorado .unnumbered}

A demora do processo de entrega acaba frustrando os desenvolvedores
devido a longa espera e *feedback* lento (EP\_35). O principal fator que
causa demora no processo de entrega devido as atividades de testes, além
da execução de etapas manuais (EP\_03). Em uma arquitetura de
microsserviços essa demora pode se tornar um gargalo, se houver poucas
instâncias do servidor e muitas versões de serviços diferentes a serem
lançadas, quando as instâncias estiverem ocupadas as novas solicitações
serão inseridas uma fila para serem executadas posteriormente.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_35** – *“At the same time the problem was severe in terms of
    wall-clock time lost just waiting for a build/release.”*

### Infraestrutura {#infraestrutura .unnumbered}

Nesta seção, serão examinadas as dificuldades relacionadas à
infraestrutura necessária para implementar práticas contínuas.

#### D30. Configuração Manual de Software {#d30.-configuração-manual-de-software .unnumbered}

A configuração manual da aplicação em produção representa um desafio
para o sucesso do , devido a ser processo complexo e sujeito a erros de
configuração. Shahin et al. (EP\_14) elenca dois outros motivos para se
ter configuração manual e provisionamento: (i) falta de ferramentas
maduras; e (ii) não tem muito valor em automatizar a configuração e o
provisionamento.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“[...] several of the interviews’ and survey
    participants have said that manual configuration of complex
    software, particularly when there is a tight coupling between
    software and hardware, and regulatory environments represented a
    significant obstacle to CD success.”*

#### D31. Falta de Recursos {#d31.-falta-de-recursos .unnumbered}

A necessidade de recursos pode ser um bloqueador para empresas menores
devido ao seu custo. Laukkanen et. al (EP\_32) exemplificam o desafio
enfrentado por uma *startup* que por causa da falta de recursos, não
tinha nenhum ambiente de teste semelhante ao de produção para
verificação interna do produto.

A falta de recursos pode levar a uma competição devido as equipes
precisarem compartilhar a infraestrutura de compilação, caso a
capacidade computacional suficiente para suprimir a demanda toda a
empresa (EP\_35).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_32** – *“The lack of resources was visible in that the
    organization did not have any production-like test environment for
    internal verification of the product.”*

-   **EP\_35** – *“If both agents were busy with a current build or
    release, then any more requests would just get queued, and the queue
    itself would start growing.”*

#### D32. Esforço Inicial {#d32.-esforço-inicial .unnumbered}

No início da adoção um um esforço inicial é necessário para configurar o
sistema de e monitorá-lo. De acordo com @Laukkanen2017, o esforço
inicial percebido para implementar o sistema de pode causar uma situação
em que se torna difícil motivar as partes interessadas para a adoção das
práticas /.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_05** – *“No início da adoção do processo é necessário um
    esforço inicial para configurar as ferramentas, treinar a equipe e
    implantar os subprocesso, o que irá gerar um grande impacto na
    velocidade do desenvolvimento e manutenções durante o início da
    adoção do processo.”*

<span>lllc</span> [tbl:desafios~p~ipeline]\

& & &\

& & &\
 & & EP\_14 &\
 & & EP\_28, EP\_36 &\
 & & EP\_21 &\
 & & EP\_33 &\
 & & &\
 & & EP\_33 &\
 & & EP\_19, EP\_28 &\
 & & EP\_25, EP\_42 &\

& & EP\_21, EP\_52 &\
 & & EP\_33 &\

& & EP\_21 &\
 & & EP\_35 &\

& & EP\_35, EP\_36 &\

& & EP\_03, EP\_07 &\
 & & &\
 & & EP\_05, EP\_25 &\

& & &\
 & & &\
 & & EP\_14 &\

& & EP\_25 &\
 & & &\
 & & EP\_14, EP\_25 &\
 & & EP\_14 &\
 & & EP\_25, EP\_33 &\
 & & EP\_14 &\
 & & EP\_33 &\

& & EP\_14 &\
 & & EP\_03, EP\_35 &\

& & EP\_14 &\
 & & &\
 & & EP\_05 &\

### Q2. Que práticas foram relatadas para implementar com êxito práticas contínuas? {#subsec:srl_rq3_praticas}

Esta questão buscou encontrar boas práticas adotadas para implementar
práticas contínuas. A partir das evidências coletadas pela revisão
sistemática, 20 Melhores práticas a serem adotadas no pipeline de
implantação foram identificadas. Essas práticas são descritas abaixo e
sumarizadas pela .

### MP1. Adoção de Práticas Ágeis {#mp1.-adoção-de-práticas-ágeis .unnumbered}

As práticas ágeis mantêm as equipes em um ritmo constante de produção e
de entrega das funcionalidades e são vistas como boas para incentivar a
adoção de integração e entrega contínua. Vassallo et al. (EP\_06)
declaram que a introdução de um pipeline de CD impõe um processo de
desenvolvimento ágil para reduzir o esforço e a duração de teste e
implantação. Dentre as várias práticas existentes, foram mencionados os
métodos Scrum (EP\_06, EP\_28, EP\_45, EP\_49), Kanban (EP\_28, EP\_42,
EP\_45, EP\_49), (EP\_25, EP\_45) e Lean (EP\_28, EP\_45).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“The next step was the introduction of a CD pipeline
    enforcing an agile development process to reduce the testing and
    deployment effort and duration, especially because such activities
    were used to be mainly manual work for two separate teams.”*

-   **EP\_28** – *“Agile, lean practices (and their adaptations): No
    explicit agile method in cases, except for Case B, which was using
    Scrum. However, implicit adaptation to agile Scrum and lean Kanban.
    From Scrum practices, e.g., daily/weekly stand-up meetings,
    retrospectives and task estimation. From lean, task tracking and a
    Kanban board were used in all cases. Rationale for not using Scrum
    in its entirety was to be more efficient and less constrained to the
    procedures.[...] Our findings show toolchain use and support for the
    activities of the deployment pipeline in all cases, while also
    applying the principles and practices of trunk-based development,
    code reviews, CI and Agile and lean.”*

-   **EP\_42** – *“Moreover, an open-minded team can be easily
    influenced to adopt the required development practices. For example,
    we ask new teams to use Kanban, Test Driven Development (TDD) (Beck,
    2002), Behavior Driven Development (BDD) (Wynne and Hellesoy, 2012),
    and other, similar development methodologies.”*

-   **EP\_45** – *“The popularity of continuous integration is
    facilitated by the explicit recommendation of the practice in the
    Extreme Programming agile method (Beck, 2000), and indeed the
    practice is highly compatible with the frequent iterations of
    software produced by agile approaches.”*

-   **EP\_49** – *“Adopting Scrum and Kanban practices Separating larger
    projects and “fast lane” development.[...] The development method
    evolved first into Scrum practices and three month sprints, and
    further separating a specific “fast lane”, separate from longer
    projects, by applying a Kanban approach to implementing and
    deploying certain tasks more rapidly.”*

### MP2. Padronizar o Fluxo de trabalho no Sistema de Controle de Versões {#mp2.-padronizar-o-fluxo-de-trabalho-no-sistema-de-controle-de-versões .unnumbered}

Ter o código fonte versionado é uma das primícias das práticas
contínuas, no entanto, adotar a prática de versionamento sem tem ter um
fluxo de trabalho definido pode dificultar a implantação contínua.
Lwakatare et al. (EP\_28), Ivanov e Smolander (EP\_29) sugeriram em seus
estudos a padronização do fluxo de trabalho dos sistemas de controle de
versão utilizando o *Trunk-Based Development* (TBD) e o *Git Flow*,
respectivamente.

***Git Flow*** ou Fluxo de trabalho Git, um modelo de organização de
branches criado por Vincent Driessen[^1] que sugere que sejam criadas 4
ramificações além da principal sendo elas: (i) *master*: contém o código
em nível de produção; (ii) *develop*: contém o código em nível
preparatório para o próximo implantação, ou seja, quando as novas
funcionalidades são terminadas, elas são juntadas com esta *branch*;
(iii) *feature branches*: são branches criadas pra desenvolver um novo
recurso; (iv) *release branches*: *branch* com um nível de confiança
maior do que a *branch develop*, se encontrando em nível de preparação
para ser mesclada com a *branch master*, caso tenha ocorrido alguma
correção de bug nesta *branch*, com a *develop*; e (v) *hotfixes*:
branches no qual são realizadas correções de bugs críticos encontrados
em ambiente de produção, e que por isso são criadas a partir da branch
master, e são juntadas diretamente com a branch master e com a *branch
develop* @Driessen:2010.

Driessen (2010) adicionou uma nota em seu artigo em que sugere adotar um
fluxo de trabalho mais simples do que o seu, para aplicativos web e
equipes está adotaram entrega contínua de software.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_39** – *“The model uses so-called feature branches. There are
    a develop branch with the latest development changes merged from
    feature branches, release branches with the version ready for
    internal testing and a master branch with a stable production-ready
    version.[...] The Git workflow model suggests that the developer
    checks out the code and creates a feature branch. The input to the
    pipeline is a commit to the feature branch. After the local
    development and testing, the changes from the branch are committed
    into the repository.[...] The reason for this is that commits into
    the release branch are done less often than to the develop branch.
    It is assumed that the develop branch will receive five merge
    requests per day and the release branch only one merge request per
    two weeks. The changes in the release branch are deployed for
    internal testing conducted by the end users within the company.”*

***Trunk-based development*** () ou em português Desenvolvimento
baseando em troncos, é um modelo de ramificação do sistema de controle
de versão, onde os desenvolvedores colaboram em código em um único
*branch* chamado “tronco” (*master* no Git), resistindo a qualquer
pressão para criar ramificações de desenvolvimento de longa duração
@Hammant:2017.

Esse fluxo de trabalho facilita a adoção de práticas contínuas, como
integração e entrega contínua, pois diferentemente de outros fluxos que
adiam a integração da *feature* até que esteja completa, orientando a
construção de pequenos lotes de códigos que devem ser integrados
frequentemente para eliminar integrações longas (EP\_28).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_28** – *“Trunk-based development: Frequent merges of branches
    to the mainline in all cases to minimise effort and conflicts
    resulting from code merges. In Case D, feature branches were
    released and thus maintained for some APIs. [...] Our findings show
    toolchain use and support for the activities of the deployment
    pipeline in all cases, while also applying the principles and
    practices of trunk-based development, code reviews, CI and Agile and
    lean.”*

### MP3. Mudanças do Esquema do Banco de Dados no Sistema de Controle de Versão {#mp3.-mudanças-do-esquema-do-banco-de-dados-no-sistema-de-controle-de-versão .unnumbered}

Quando se desenvolve software com um banco de dados , as novas
funcionalidades podem exigir que sejam realizadas alterações no banco de
dados. Essas alterações pode ser adicionar uma nova coluna ou correções
de dados. Ivanov e Smolander (EP\_39) classificou a prática de versionar
as mudanças do esquema de banco de dados como uma das 25 praticas
importantes de 27 práticas sugeridas de automação DevOps.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_39** – *““Version control DB [database] schema changes” (\#27)
    was called as an important practice for relational databases but in
    the context of the case project and its schemaless database this
    practice was also marked as not important.”*

### MP4. Todos os commits estarem vinculados às tarefas {#mp4.-todos-os-commits-estarem-vinculados-às-tarefas .unnumbered}

Toda a mudança no código deve estar relacionada a alguma tarefa, tornado
as mudanças parte de um plano geral. Além de gerar rastreabilidade nas
mudanças que podem ser usadas posteriormente em uma auditoria ou
documentação, permitindo o acompanhamento do ritmo da equipe. Ivanov e
Smolander (EP\_39) categorizaram essa prática como sendo relacionada ao
sistema de controle de versão e como uma das 27 práticas sugeridas de
automação DevOps.

### MP5. Commit de código com mais frequência {#mp5.-commit-de-código-com-mais-frequência .unnumbered}

A prática de “commitar frequentemente” alinhada com a prática de
“commits pequenos” contribuem diretamente para o cerne do integração
contínua que é o feedback rápido, pois ao fazer commits menores e com
mais frequência, é reduzido o esforço de depuração e os programadores
podem resolver mais bugs e problemas (EP\_27, EP\_34). Rahman et al.
(EP\_34) afirmam que apenas a adoção de pode não ser suficiente para
colher os benefícios de uso e nem melhorar o processo de desenvolvimento
de software, pois para que isso aconteça se faz necessário que os
desenvolvedores adotem as melhores práticas de CI, como por exemplo, a
prática de commits frequentes.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_27** – *“Continuous integration encourages developers to
    “break down their work into small chunks of a few hours each”, as
    smaller and more frequent commits helps them keep track of their
    progress and reduces the debugging effort [15], [16].”*

-   **EP\_31** – *“[...] the team has identify the practice of “commit
    often, commit little” as important - they commit small code
    increments (e.g. 10-20 lines of code) and do that very often.”*

-   **EP\_34** – *“The programmer utilizes this feedback [provided by
    the CI tool in case the build fails] to fix the code changes by
    making more commits, fixing their code changes, eventually leading
    to more bug fixes and issue completions. Hence, by making more
    commits, programmers might resolve more bugs and issues.[...] The
    Practice of Making Frequent Commits: Our findings suggest that only
    adoption of CI tools may not be enough to reap the benefits of CI.
    [...] Our findings suggest that to reap the benefits of CI usage,
    practitioners should also apply the best practices of CI such as,
    making frequent commits.”*

### MP6. Commits pequenos {#mp6.-commits-pequenos .unnumbered}

Como mencionado na anteriormente as prática de “commits frequentes” e
“commits pequenos” favorecem que os desenvolvedores colham os beneficios
de adotar , como por exemplo. o feedback rápido (EP\_34). Zhao et al.
(EP\_27) afirmam que com a diminuição da quantidade de códigos do commit
e o aumento de sua frequência, facilita o processo de verificação do
build, bem como a prática de revisão de código através do *pull
request*.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_27** – *“the “commit small” guideline, however, is followed
    only to some extent, with large differences between projects in
    terms of adherence to this guideline; [...] The expected decrease in
    the size of the commits is also echoed by one of the survey
    respondents: “commits became smaller and more frequent, to check the
    build; pull requests became easier to check” (R4).[...] the
    decreasing trend in commit churn is also consistent with the
    observation that as projects age, bug-fixing commits, which on
    average are smaller, become more common than new-feature commits,
    which on average are larger [35].”*

-   **EP\_31** – *“[...] the team has identify the practice of “commit
    often, commit little” as important - they commit small code
    increments (e.g. 10-20 lines of code) and do that very often.”*

-   **EP\_37** – *“The authors [Ståhl e Bosch (2014) e Zhao et al.
    (2017)] observe that practices such as “commit often” and “commit
    small” are indeed employed after the adoption of CI. However, the
    growing trend of closed issues slow down after the adoption of CI.”*

### MP7. Trabalhar em Pequenos lotes {#mp7.-trabalhar-em-pequenos-lotes .unnumbered}

Para que a equipe de desenvolvimento tenha uma rápida progressão da
etapa de desenvolvimento para a produção, por meio de testes e operações
se faz necessário trabalhar com código em pequenos lotes.

O lote é a unidade de trabalho que se move através do fluxo de trabalho
ou fluxo de valor. Quanto menor um lote de trabalho mais rápido chegará
à próxima etapa ou será entregue ao cliente, reduzindo o tempo de ciclo
e fazendo os desenvolvedores obterem feedback mais rápido, pois o código
produzido é revisado em cada etapa.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_15** – *“[...] encouraged DevOps practices such as fast
    feedback, small batch sizes, and independent releases, emphasizing
    increased team autonomy”*

### MP8. Refatoração {#mp8.-refatoração .unnumbered}

Refatoração, segundo Fowler (2018), “é o processo de mudar um sistema de
software de uma forma que não altere o comportamento externo do código,
mas melhore sua estrutura interna.” As principais razões para refatorar
incluem melhorar a compreensão do programa, permitir fazer alterações
mais fáceis e ajudar a encontrar bugs. A refatoração pode ser realizada
em conjunto com outras tarefas ou de forma separada das demais tarefas.

O estudo indica que as tarefas de refatoração são geralmente programadas
de maneira adequada, os que não o fazem alegam que consome muito tempo,
reduz o esforço de tarefas de implementação de recursos ou que não
perceberam claramente as vantagens da refatoração.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“[...] refactoring is usually properly scheduled. The
    main reasons for refactoring include improving program comprehension
    (87%), allow making changes easier (77%), and help to find bugs
    (24%).Those who not schedule refactoring tasks, they do it either
    because they are too time consuming and take effort away from
    feature implementation tasks (27%), or because they do not clearly
    perceive refactoring advantages (9%).[...] Differently from what
    Fowler reported [25], refactoring tasks are often performed together
    with other tasks[...]”*

### MP9. Revisão de Código {#mp9.-revisão-de-código .unnumbered}

A revisão de código tem objetivos bem claros detectar *bad smells* e
encontrar defeitos, compartilhar o conhecimento do código, os estilos e
padrões de codificação, encontrar maneiras alternativas de implementar
um recurso, garantir a qualidade. Os fatores considerados importantes na
revisão do código incluem o conhecimento do revisor, o tamanho das
alterações no código a serem revisadas e o suporte do ambiente de
revisão.

A revisão de código geralmente é realizada através de *pull request* pra
mesclar um *branch* de trabalho ao *branch master*. Nesse momento, os
revisores do código verificam as mudanças, dão feedback crítico e
sugeriram se as mudanças deveriam ou não ser aceitas para o produto. O
desenvolvedor pode melhorar as mudanças no *branch* com base no feedback
e até que seja corrigido, os revisores não o aprovam. O *brach* de
trabalho também foi continuamente testado pelo sistema de e não seria
integrado ao produto se todos os testes não fossem aprovados (EP\_32).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“[...] the obvious purposes are detecting bad smells
    (90%) and finding defects (81%). However, code review is also used a
    lot to share code knowledge (85%), or to find alternative ways for
    implementing a feature (75%).”*

-   **EP\_28** – *“Main purpose was to ensure quality and an opportunity
    to share information about coding styles and standards. Factors in
    code review considered important included knowledge of the reviewer,
    size of code changes to be reviewed and review environment
    support.”*

-   **EP\_32** – *“BigCorp, however, did not have a formal code review
    practice in place and was struggling with low quality code partly
    because of that.[...] There was no clear reason why code review was
    not practiced. Due to the lack of code review and a high number of
    new and inexperienced developers, there were signs of bad code
    quality.[...] Developers worked in feature branches during
    development. When a piece of work was thought to be ready, a pull
    request was opened and a lead developer and a few other developers
    were assigned to it. The assignees reviewed the changes, gave
    critical feedback and suggested whether or not the changes should be
    accepted to the product. The developer could improve the changes in
    the branch based on the feedback. The branch was also continuously
    tested by the CI system and it would not be integrated to the
    product if all the tests would not pass.[...] The code review
    process had multiple benefits for SmallOrg. First, all code changes
    were reviewed by experienced lead developers, which helped
    onboarding new developers and prevented low quality code from
    entering the product. Second, the changes were not integrated into
    the product until the code review was completed and the CI build
    would pass for the feature branch. Thus, the product build was green
    almost all the time, as build-breaking changes would not be accepted
    for integration.”*

-   **EP\_39** – *“A code review should be conducted after submitting a
    merge request and before merging.”*

-   **EP\_50** – *“Code reviews are prevalent in continuous deployment
    processes. Because developers are fully responsible for the entire
    lifecycle of the software, code reviews are taken more seriously and
    there is far less resistance to them.”*

A ***peer-review*** ou revisão por pares é um tipo de revisão de
software em que o código produzido é revisado por outro desenvolvedor,
com a finalidade de detectar e corrigir defeitos além de avaliar a
qualidade. Ivanov e Smolander (EP\_39) listaram a revisão por pares como
uma sugerida de automação DevOps, classificando-a como teste e controle
de qualidade.

### MP10. Análise Estática de Código Automática {#mp10.-análise-estática-de-código-automática .unnumbered}

A análise estática automática complementa o , pois o uso de ferramentas
que fazem essa análise auxiliam os desenvolvedores a testarem o seu
código sem realmente executá-lo, encontrando falhas de programação,
vulnerabilidades, *bad smells* (indicador de um possível problema
estrutural em código-fonte, que pode ser melhorado via refatoração
@fowler2018refactoring), verificando se os desenvolvedores estão
cumprindo as diretrizes de codificação e etc, que poderiam ir para o
cliente.

Com o uso de ferramentas automatizadas de análise de código estático no
, esses problemas encontrados são encontrados antes de a versão ser
lançada. Essas ferramentas produziriam avisos que todos veriam e em
alguns casos produzindo quebras de *build*. E ao mesmo tempo, no
entanto, tal efeito sugere que o uso dessas ferramentas com prudência
ajuda a evitar muitas quebras de compilação desnecessárias.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_04** – *“[...] the use of ASCATs in CI produces a “stronger”
    message in case the tool reveal warnings, letting everybody be aware
    about the issue and, in some cases, producing build breakages. At
    the same time, however, such an effect suggests an use of ASCATs
    with parsimony to avoid many unnecessary build breakages.”*

-   **EP\_06** – *“Respondents indicate (Q2.5) that code reviews are the
    premier way for detecting code smells (92%), while 63% of the
    respondents also use static analysis tools. ”*

### MP11. Coleta de méticas de qualidade {#mp11.-coleta-de-méticas-de-qualidade .unnumbered}

A qualidade é interpretada e entendida de maneira diferente por cada um.
Os desenvolvedores coletam métricas para o monitorar a qualidade do
código produzido, algumas dessas métricas são a quantidade de código
duplicado, que tradicionalmente também é considerada uma espécie de
cheiro ruim, a complexidade ciclomática, número de parâmetros de função
e *Lines of Code* (LOC).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“[...] developers collect a series of metrics to
    monitor source code quality (Q2.8). The main metrics used are
    reported in Fig. 8. Surprisingly, the most important metric is the
    amount of duplicated code (78%) which traditionally is considered as
    a kind of bad smell too. Other than that, the cyclomatic complexity
    (69%, again, indicator of some code smells such as Complex Method)
    and number of function parameters (51%,indicator of Long Parameter
    List bad smell). Only 44% of respondents mention LOC”*

### MP12. Testes automatizados {#mp12.-testes-automatizados .unnumbered}

O teste automatizado é um fator importante que afeta a relação
custo-benefício da integração contínua, pois os testes estão intimamente
relacionada a ela, logo, sem tais testes não deve ser considerado IC de
forma alguma (EP\_27). Zhao *et.al* (EP\_27) diz que a é frequentemente
introduzida juntamente com a automação de testes.

A adoção de testes automaticos contribui como um impacto positivo na
qualidade geral do código de produção, permitindo implantações mais
rápidas e com alta qualidade (EP\_28, EP\_46, EP\_49). Itkonen et al.
(EP\_49) identificaram o teste automático como um dos fatores causam a
diminuição do risco de liberação e implantação dos aplicativos, pois os
testes reduziram o risco de descobrir bugs após as implantações de
produção.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_27** – *“Automated testing is an important factor that affects
    the cost-effectiveness of CI and much effort has been devoted to
    improve the quality and efficiency of automated testing in CI.”*

-   **EP\_28** – *“Automation in testing and deployment contributed to
    the positive impact on the overall quality of the production code.”*

-   **EP\_46** – *“Automated Testing: The artifact that is generated in
    the previous stage [commit] is deployed to a testing environment.
    Automatic testing is done for all aspects of the software. The
    environment is also provisioned and configured automatically. If the
    tests fail, this artifact does not progress any further.”*

-   **EP\_49** – *“From the perspective of the customer’s architect,
    many changes had contributed to the fact that the quality has
    increased. Considerably less bugs after production deployment is
    attributed to the adoption of automated testing, static code
    analysis, production-like environments in the deployment pipeline,
    and major refactoring and platform improvement projects.”*

### MP13. Definir Estratégias de testes {#mp13.-definir-estratégias-de-testes .unnumbered}

As estratégias de teste servem para guiar a equipe de desenvolvimento a
um objetivo em comum: eliminar o máximo possível de bugs e desvios de
implementação. Os desenvolvedores usam estratégias de teste específicas
raramente ou não usam nenhuma estratégia, porém dependendo do recurso em
teste, eles escolhem qualquer estratégia é a mais adequada. Quanto ao
nível de cobertura os desenvolvedores que tentam atingir pelo menos 80%.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“We found that developers make use of specific testing
    strategies such as black box testing relatively seldom (Q3.5). 52%
    of the respondents say they do not use any strategy.[...] Most of
    the respondents picked multiple options [criteria white box testing]
    indicating that depending on the feature under test, they choose
    whichever strategy is most suitable.[...] Overall, about statement
    coverage (Q3.12), 84% of the respondents indicated they try to
    achieve a coverage level of at least 80%.”*

### MP14. Melhorar a atividade de teste {#mp14.-melhorar-a-atividade-de-teste .unnumbered}

Essa seção discute 17 práticas propostas na literatura para melhorar a
fase de teste durante a . Vassallo et al., Amrit e Meijberg (EP\_06,
EP\_08) sugerem que o uso da prática de desenvolvimento ***Test Driven
Development* ()** indicam um aumento na qualidade do código juntamente
com um efeito inconclusivo na produtividade do desenvolvedor, pois
facilita a localização de mais defeitos (*Defect Reduction*) e também na
redução do tempo necessário para corrigir os defeitos (*Defect lead and
throughput*).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“Generally, our survey answers suggest that quality
    assurance through testing is a crucial concern at ING NL.[...] The
    majority of developers mention they use TDD, although we do not know
    whether they are strictly applying TDD. At the same time, quality
    assurance in the form of (manual) testing requires a significant
    portion of the allocated time for a sprint.”*

-   **EP\_08** – *“The outcomes of the empirical studies of TDD
    implementation seem to indicate an increase in code quality along
    with an inconclusive effect on developer productivity[...] Though
    the inferential statistics are not conclusively in favor of the TDD
    and CI case (CS2), the descriptive statistics point to an overall
    improvement in not only finding more defects (Defect Reduction), but
    also in shortening the time required to fix the defects (Defect lead
    and throughput).”*

Vassallo et al. (EP\_06) explica que os desenvolvedores confundem o
conceitos de ***Behavior Driven Development* ()** e , no entanto, o é
uma técnica de desenvolvimento de software, onde os programadores
desenvolvem o software direcionados por comportamentos, deferente do
Chen (EP\_42) que sugerem que as duas técnicas de desenvolvimento sejam
executadas em conjunto.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_06** – *“Casual evidence from another context (not at ING NL)
    suggests that, some developers were referring to acceptance testing
    with the Framework for Integrated Testing (FIT) [36] as TDD, but
    meant Behavior-Driven Development (BDD) [37].”*

-   **EP\_42** – *“For example, we ask new teams to use Kanban, Test
    Driven Development (TDD) (Beck, 2002), Behavior Driven Development
    (BDD) (Wynne and Hellesoy, 2012), and other, similar development
    methodologies.”*

No estudo, Chen (EP\_42) defende a **inclusão das verificações de
segurança automatizadas** em um pipeline , sendo executada nos estágios
iniciais, produzindo uma trilha de auditoria das alterações feitas para
cada confirmação de código, incluindo quando a varredura de segurança
foi conduzida, o que foi verificado e quais foram os resultados da
verificação. Shahin et al. (EP\_14) complementam informando que tal
prática alivia a preocuxapação dos lideres de negócio quanto nível de
qualidade do produto de software, tornando o pipeline atraente para
eles.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“Whilst the main business leaders’ concern is around
    quality level, our results suggest that integrating automated
    quality checks and security test in both development and operations
    processes can alleviate this concern and to a large extent make
    continuous deployment compelling to business leaders.”*

-   **EP\_42** – *“With CD, the execution of security checks is
    automated. The automation is built into one of the early stages of
    the CD pipeline. Thus, every code commit goes through the security
    check.”*

Os **testes unitários** são testes de caixa branca que verificam a
lógica das unidades () alvo, sendo executados para cada commit do código
(EP\_20, EP\_28, EP\_39, EP\_42). As unidades podem ser métodos,
classes, funcionalidades, módulos e etc. Mårtensson, Ståhl e Bosch
(EP\_30) afirmam que os testes desse tipo são vistos como “ferramentas
de desenvolvedor” e devem ser executados pelos desenvolvedores antes de
commitar o código e usados como teste de regresão. Shahin, Babar e Zhu
(EP\_21) afirmam que se os testes unitários forem mal elaborados e mal
escritos, esses se tornar testes de longa execução ocasionando um
aumento no tempo de ciclo do pipeline de implantação, bem como a
diminuição do ciclo de feedback.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“Unit tests: These white-box tests primarily verify
    the logic of target units. Limited unit tests are run manually on
    the development environments, XCode or Android Studio, using tools
    such as XCTest [11], JUnit [12], or Robolectric [13]. More extensive
    as well as automated unit tests are run on serverbased simulators.”*

-   **EP\_21** – *“Long running tests can increase the cycle time (i.e.,
    the time needed to transfer code from code repository to production)
    of continuous deployment pipeline as well as slow down the feedback
    cycle in deployment pipeline. That is mainly because tests are
    poorly designed and written. For example, a participant reported
    that they were able to address the slow cycle of feedback from
    continuous deployment pipeline by applying two approaches: (i)
    creating much smaller unit tests, in which gave them immediately
    feedback;[...]”*

-   **EP\_28** – *“Unit tests are executed as part of build process and
    SonarCube is used for checking code coverage.”*

-   **EP\_39** – *‘The implemented DevOps pipeline fulfils all the
    requirements identified in RQ1. The pipeline includes all of the
    practices selected in the workshop on DevOps automation of the case
    project and ensures high quality of the code through unit tests,
    code quality check tools and end-to-end testing [33].’’*

-   **EP\_42** – *“Unit tests are executed for every code commit.
    Acceptance tests are executed for each code commit that passes the
    unit tests.”*

O **teste de integração** é um tipo de teste de caixa preta que sucede o
teste unitário e têm por objetivo encontrar falhas de integração entre
as unidades. Portanto, o principal trabalho realizado pelas ferramentas
de CI é validando do código produzido através da execução dos testes
unidade e de integração (EP\_28, EP\_36).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“Integration tests: These standard (blackbox)
    regression tests test key features and key flows of the app. They
    typically run on simulators and are not necessarily device
    specific.[...] As one might expect, FB [Facebook] applies numerous
    types of tests, including unit tests, static analysis tests,
    integration tests, screen layout tests, performance tests, build
    tests, as well as manual tests.”*

-   **EP\_21** – *“. All the participants believed that they were able
    to automate the units and integration tests to a large extent
    [...]”*

-   **EP\_28** – *“A CI server validates the code with unit and
    integration tests and stores a Debian package to an internal
    repository.”*

-   **EP\_36** – *“For CI builds, the main work done by the CI tools is
    integration testing, so we parsed the CI build scripts8 to
    distinguish between deployment builds (the aim of this CI build is
    to deploy images) and general test builds.”*

**Teste de cobertura** é uma métrica em testes de software capaz de
medir a quantidade de testes realizados por um conjunto de testes em
toda a base de código. Humble e Farley (2014) definem que a cobertura de
testes deve ser de no mínimo 75% de toda a base de código, afim que de
os desenvolvedores tenham um bom grau de confiança do funcionamento da
aplicação, já para Chen (EP\_17) o ideal é, no mínimo, 90% de cobertura,
caso contrário, o pipeline do implantação falhará na compilação.

Quando inserida no pipeline de implantação a equipe pode estipular um
valor mínimo de cobertura de testes que o código deve ter (EP\_32), caso
a cobertura seja menor que a estipulada a o pipeline do falhará na
construção (EP\_17).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_17** – *“Test code is reviewed as rigorously as application
    code. For any code change, if the test coverage (both line and
    condition) is below 90%, the CD pipeline will fail the build.”*

-   **EP\_32** – *“BigCorp had put plenty of resources to verify the
    quality of their product before giving it to the customers. First,
    the organization had dedicated testers that created automated test
    cases but also performed manual testing on the product. Second, the
    organization had a definition of done that included test coverage
    criteria for automated tests.”*

Os ***smoke test*** ou teste de fumaça mencionado nos estudos (EP\_15,
EP\_32) são um subconjunto de testes que são executados rapidamente com
frequência, em vez de executar suítes de teste mais extensas, que
levariam mais tempo para serem executadas. Os teste de fumaça cobrem as
funcionalidades mais importantes, sendo usado para avaliar se tais
funcionalidades parecem estar funcionando corretamente (EP\_32).
Callanan e Spillane (EP\_15) dizem que esses testes podem ser usados
para monitorar ferramentas a serem executadas ou para o pessoal de
operações usar durante a manutenção ou solucionar problemas.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_15** – *“The script was a simple Linux shell script named
    smoketest.sh that assumed the service it was testing was already
    running on localhost, indicating failure via a nonzero exit code if
    errors occurred.[...] Smoke tests were to be “nondestructive”— that
    is, using read-only access or writing only to previously approved
    test data. These tests were also available for monitoring tools to
    execute or for operations staff to use during maintenance or
    firefighting.”*

-   **EP\_32** – *“[...] that early in the development, SmallOrg did not
    focus on unit testing at all and they had increased the coverage
    only afterwards. Instead of aiming at a high test coverage, SmallOrg
    had created smoke tests which allowed fast verification that nothing
    was critically broken.”*

***Build test*** ou testes de compilação é um conjunto de testes que são
executados para determinar se o código foi compilado corretamente
(EP\_20). Além de serem executados diversos tipos de teste como testes
de unidade, testes de integração, *smoke test*, o teste de compilação
pode ser executado para garantir que a construção com as novas
alterações funcione corretamente. Esses testes podem ser usados quando
uma compilação completa consome muito tempo e recursos apenas para
testar as dependências com alguns níveis de profundidade (EP\_20).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“As one might expect, FB applies numerous types of
    tests, including unit tests, static analysis tests, integration
    tests, screen layout tests, performance tests, build tests, as well
    as manual tests.[...] Moreover, a test is run to ensure a build with
    the changes works correctly. However, since a full build is time and
    resource intensive, the build test here only tests dependencies a
    few levels deep.”*

O **teste de regressão** é uma técnica de teste de software que consiste
na execução de algum subconjunto de testes para garantir que a adição de
uma nova funcionalidade não gere defeitos em funcionalidades já testadas
e que não sofreram modificações. Em um pipeline de implantação os testes
de regressão passam a ser o conjunto de testes automatizado que
executado toda vez que um código é commitado garantindo que não propagou
nenhum defeito ao código pré-existente.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“Integration tests: These standard (blackbox)
    regression tests test key features and key flows of the app. They
    typically run on simulators and are not necessarily device
    specific.”*

-   **EP\_26** – *“Nightly regression testing of core functionality kept
    pace with development and supported both functional testing and
    system-to-system integration. As defects were found in end-to-end
    business scenarios, responsive resolutions were managed in hours or
    days, not the weeks typical for larger enterprise systems.”*

**Testes de sistema** são testes caixa preta realizados em um sistema
integrado completo para avaliar se está em conformidade com os
requisitos. No pipeline de implantação esse tipo de teste é executado
depois dos testes de unidade e de integração, seguindo essa ordem
(EP\_30). Mårtensson, Ståhl e Bosch (EP\_30, apud Rathod e Surve, 2015)
disseram que só por meio dos testes de sistema que a qualidade e
segurança de um produto de software pode ser garantida.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_30** – *“Rathod and Surve present a different approach: “It is
    only through efficient system testing that the quality and safety of
    a software product can be guaranteed.”[...] Unit/component tests
    followed by system tests to check the developers’ software changes.
    System tests of vital functions (eg, start up the system or drive
    around) secure stability and integrity in the system, which is
    monitored by, eg, a test manager or QA department.”*

Os **testes de aceitação** tem como objetivo validar se as
funcionalidades do produto estão de acordo com os requisitos e processos
de negócios do usuário para determinar se o sistema satisfaz ou não os
critérios de aceitação estabelecidos (EP\_15, EP\_42). Esses testes
devem ser executados em um ambiente similar ao de produção, no entanto,
dependendo das configurações específicas do ambiente de produção, isso
pode dificultar a construção dos ambientes de testes (EP\_16, EP\_21).

Além disso, Lwakatare et al. (EP\_16) dizem que a falta cobertura de
teste de aceitação totalmente automatizada, exigirá que muito tempo seja
gasto em teste de aceitação manual.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_15** – *“The compliance tests would run on every commit,
    during deployment to the acceptance test environments, blocking that
    release candidate if it didn’t meet one or more of the standards
    criteria.”*

-   **EP\_16** – *“[...] prior to product launch, acceptance testing is
    conducted with the customer to validate product functionality in a
    production environment.[...] Moreover, companies lack fully
    automated acceptance test coverage, requiring a lot of time to be
    spent on manual acceptance and regression testing.[...]
    Customer-specific configurations further complicate the construction
    of representative test environments for system and acceptance
    testing.”*

-   **EP\_21** – *“automating user acceptance test remains a big
    challenge and it takes a lot of workload in the company “… they
    often have a really challenges to get [automated test] done, for
    acceptance tests most of time it is not easy to fully automate”
    P9.”*

-   **EP\_42** – *“While unit tests and acceptance tests have been
    extensively discussed and widely practiced in CD, testing
    non-functional requirements has received considerably less
    attention. However, unit tests and acceptance tests are mainly
    intended to ensure functional requirements.[...] Acceptance tests
    are executed for each code commit that passes the unit tests.”*

**Teste funcional** é uma técnica de teste de software do tipo caixa
preta usada para validar se o sistema foi construido conforme os
requisitos especificados. Diferentemente do teste de aceitação que é
considerado uma atividade de validação, pois garante ao cliente que o
produto construido atende as suas necessidades, o teste funcional é uma
atividade de verificação e servindo como garantia à equipe de
desenvolvimento de que a aplicação funciona corretamente.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_29** – *“One of the interviewees (P12) described how improving
    the quality of tests could help to accelerate the feedback cycle in
    the CD pipeline. He highlighted two practices: (i) designing smaller
    test units that result in immediate feedback, (ii) decreasing the
    number of functional tests.”*

Callanan e Spillane (EP\_15) mencionam o **teste de recuperação de
desastre** como sendo um tipo de teste não funcional. Esses testes
verificam a capacidade do software se recuperar de falhas de software,
hardware, falhas de rede, entre outras.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_15** – *“Other forms of nonfunctional testing, such as
    security testing and disaster recovery testing,[...]”*

O ***snapshot test*** é usado para garantir que a interface do usuário
não mudou. Esse tipo de teste gera imagens de visualizações de tela e
componentes (*snapshot*), que são comparados a um arquivo de *snapshot*
de referência armazenado ao lado do teste, pixel por pixel, falhando se
os dois *snapshots* não coincidirem (EP\_20).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“Snapshot tests: These tests generate images of screen
    views and components, which are then compared, pixel by pixel, to
    previous snapshot versions [14, 15].”*

O **teste de performance** é um tipo de teste que é realizado para
verificar o tempo de resposta de uma aplicação, identificar gargalos e
determinar a escalabilidade e confiança da aplicação levando em
consideração uma carga (EP\_50). Rossi et al. (EP\_20) declarou o teste
de performance como um dos mais importantes, no entanto, Chen (EP\_42) o
pipeline de implantação vem sendo adotado sem os testes de aceitação e
de performance.

Diferentemente de teste que avaliam os requisitos funcionais de um
sistema, o teste de performance avalia requisitos não funcionais, ou
seja, a definição dos critérios de aprovação ou reprovação desse teste
se torna dificil. Os resultados do teste de performance pode variar de
um teste para outro devido a variações inevitáveis nos ambientes de
teste, como por exemplo as condições da rede.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“As one might expect, FB applies numerous types of
    tests, including unit tests, static analysis tests, integration
    tests, screen layout tests, performance tests, build tests, as well
    as manual tests.”*

-   **EP\_42** – *“Every time the developers see the pipeline view, the
    gaps in their CD adoption are clear. For example, they can easily
    see that the acceptance and performance stages are empty. We have
    often seen developers start discussions about how they could fill
    the gaps by writing automated acceptance tests and performance
    tests.”*

-   **EP\_50** – *“After successful completion of system testing,
    performance tests are run to catch performance issues as early as
    possible. The performance tests are executed by the developers in
    non-virtual environments for reproducibility. Automated measurements
    are made and compared with historical data.”*

Os **testes de capacidade** são criados para testar se a aplicação e o
ambiente podem lidar com o número de usuários e transações a quais foram
projetados para lidar (EP\_20). Esse tipo de teste pode ajudar a
determinar quando o ambiente precisa ser reforçado para atender à
demanda.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“Capacity tests: These tests verify that the app does
    not exceed various specified capacity limits”*

O **teste de conformidade** é tipo de teste funcional, caixa-preta, que
determina se a aplicação cumpre com os padrões especificado (EP\_20).
Esses testes verificam se o produto entregue em cada fase do ciclo de
desenvolvimento está de acordo com os requisitos acordados.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_20** – *“Conformance tests: These tests verify that the app
    conforms to various requirements.”*

Lwakatare et al. (EP\_16) diz que com a adoção de práticas contínuas as
empresas passam a ter a oportunidade de verificar rapidamente se seus
novos recursos de software são úteis para os clientes e adotar práticas
como o **teste A/B** para conduzir a experimentação de recursos. O teste
A/b é uma prática uma prática em que os usuários são atribuídos
aleatoriamente a uma das duas versões: a atual e uma “desafiante”, com
modificações, com o objetivo de descobrir qual das versões apresenta
maior taxa de conversão.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_16** – *“[...] paradigm change towards continuous deployment
    gives companies the opportunity to quickly verify whether their new
    software features are useful to customers and adopting practices
    such as A/B testing to conduct feature experimentation [5]. A/B
    testing is a practice where users are randomly assigned to one of
    the two variants of the system for experimentation e.g. feature
    usage experimentation [6].[...] Web companies with DevOps practices
    not only monitor the performance of infrastructure but also conduct
    experiments regarding feature usage through A/B testing and canary
    releases [1], [2].”*

### MP15. Paralelização de Testes {#mp15.-paralelização-de-testes .unnumbered}

A paralelização de testes significa executar testes automatizados em
paralelo em vez de serialmente, fazendo com que o tempo de execução dos
testes seja reduzido. Essa prática necessitada de recursos suficientes
para executar os testes, esses podem ser executados em uma ou várias
máquinas @Laukkanen2017.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_14** – *“The participants also mentioned the need to test all
    types of applications (for example mobile testing as it is fragile
    and expensive to automate), techniques and tools that enable
    parallelization of automated testing and infrastructure automation
    testing.”*

-   **EP\_32** – *“SmallOrg had reduced the build time by building only
    components that had changed after previous run and by running tests
    in parallel.”*

### MP16. Microsserviços {#mp16.-microsserviços .unnumbered}

A arquitetura microsserviços tenta quebrar sistemas complexos em
serviços pequenos, autônomos e implantáveis de forma independente, sendo
o estilo arquitetônico inicial e promissor para práticas de . A mudança
de uma arquitetura monolítica para para uma arquitetura de
microsserviços, observa-se uma maior capacidade de implantação,
modificabilidade e resiliência à erosão da arquitetura.

Com a adoção de microsserviços sugem dificuldades no monitoramento e na
determinação de métricas úteis, colocando muita sobrecarga de operações,
se faz necessário ter uma equipe de operações madura para adotá-lo.
Portanto, não se faz necessário adotar microsserviços ou dividir de
software monolíticos em microsserviços para se adotar práticas de .

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_17** – *“[...] we moved from a monolithic architecture to a
    Microservices architecture [8]. Rather than building large
    monolithic applications, we organize systems into small,
    self-contained, singleresponsibility units that can be independently
    developed, tested, and deployed.[...]After we moved our applications
    to a Microservices architecture, we observed increased
    deployability, modifiability, and resilience to architecture
    erosion[...]”*

-   **EP\_21** – *“ It has been said that microservices architectural
    style is the first architectural style for CD practice
    [13].[...]since microservices style puts a lot of operations
    overhead in terms of like monitoring these services, and
    administrating them, it is needed to have mature operations team to
    adopt it.”*

-   **EP\_28** – *“Difficulties in monitoring, especially for
    microservice-based applications and in determining useful metrics.”*

-   **EP\_29** – *“Microservices are not required nor is breaking up a
    monolith [for CD]”*

### MP17. Build automatizado {#mp17.-build-automatizado .unnumbered}

O *build* ou compilação de um projeto é uma atividade composta por
vários passso, que inclui a compilação do código, execução de testes,
empacotamento, geração de artefatos de documentação, entre outros. Essa
atividade deve ser repetida a cada mudança realizada na aplicação.

Fazer com que os códigos fontes se transformem em um sistema em execução
pode muitas vezes ser um processo complicado se executado manualmente,
pois apresentam risco de falha devido a erro humano, portanto, tal
tarefa pode ser automatizada (EP\_48; FOWLER, 2006). A automatização do
processo de *build* é uma das principais práticas que compõe o
@Fowler:2006, e deve ser executado automaticamente a cada commit,
reduzindo o risco de compilações defeituosas devido à configuração
manual incorreta e o impacto das alterações do ambiente nas versões
existentes (EP\_39, EP\_48).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_28** – *“New merges to the master branch trigger the CI server
    to automatically build and subsequently deploy to the test
    environment, where unit tests and end-to-end tests against test
    database are executed.”*

-   **EP\_31** – *“The automated build and test processes are often
    intertwined with manual reviews and bug-fixing activities.”*

-   **EP\_39** – *“Build process is run automatically on commit.[...]
    The commit triggers the build process in GitLab that runs the code
    analysis and unit tests (\#6, 20).”*

-   **EP\_48** – *“Manual steps in any part of the development process
    introduce risk of failure due to human error. Four factors were
    identified as having decreased release and deployment risk
    significantly. First, the environment independent builds have
    mitigated both the risk of faulty builds due to erroneous manual
    configuration, and the impact of environment changes on existing
    releases.”*

### MP18. Implantação automatizada {#mp18.-implantação-automatizada .unnumbered}

A prática de autimatizar a implantação é o que permite implantar o
software em um ambiente de testes ou de produção com apenas um clique,
sendo essencial para reduzir o risco de implantações em produção e
fornecer feedback rápido sobre a qualidade do software, permitindo que
as equipes realizem testes abrangentes o mais rápido possível após as
alterações. Com a adoção dessa prática o processo torna-se repetível e
confiável (EP\_28), pois o computador passa então a executar as tarefas
de implantação sem intervenção, diminuindo os risco de falha devido a
erro humano.

O mecanismo de implantação automatizado pode ser incorporado ao servidor
de integração contínua (CI), além de poder usar diferentes estratégias
de implantação (EP\_28), como implantação azul-verde e a *rolling
upgrade*, ou implantação canária, entre outras.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_28** – *“The automated deployment mechanism can use different
    deployment strategies, but when created, it ensures the reliability
    and repeatability of system deployment [13,38].[...] Deployment
    scripts facilitated the automatic installation of software to a
    target environment by software development teams. Deployments
    scripts were mostly triggered from the CI system. Software
    developers in all cases had access and could modify the scripts,
    which were also version-controlled.”*

-   **EP\_48** – *“Also we need to automate deployment process which
    covers creating and running service containers in test environment,
    so developer and operator can test software without any extra
    effort.[...] To automate service deployment in test environment,
    test environment should exposes Docker remote API.”*

### MP19. Definir uma Estratégia de Implantação {#mp19.-definir-uma-estratégia-de-implantação .unnumbered}

No lançamento de uma versão de software ao consumidor, introduz-se o
risco de vulnerabilidades, problemas, bugs e software sem desempenho
acontecerem em produção, e portanto, havendo vários motivos para
reverter uma implantação ou produzir um *hotfix*.

Definir uma estratégia de liberação que funcione reduz o medo e o risco
de mudanças no lançamento de novos recursos para um cliente. Os autores
do (EP\_13) sugeriram diversas estratégias de implantação, as quais
serão descritas a seguir, dentre elas está a ***“Feature Flags”*** que
trata-se de uma técnica que permite que novos recurso sejam implantados
em um ambiente de produção, restringindo sua disponibilidade através de
um sinalizador, possibilitando habilitar ou desabilitar o novo recurso
para usuários específicos sem reiniciar o software ou implantar um novo
código.

-   **EP\_13** – *“Microsoft often deploys large architectural changes,
    using a combination of dark launches and feature flags. With a
    feature flag, a feature is deployed but disabled until it’s ready
    for release; the developer turns the feature off and on through a
    configuration server. This practice lets Microsoft avoid dealing
    with integration issues or maintaining long-running feature
    branches”*

Os autores (EP\_13, EP\_28) sugerem a estratégia “**implantação
canário**” que reduz o risco da introdução de uma nova versão do
software em produção, fazendo o lançamento gradual da mesma para uma
pequena parte do conjunto de usuários antes de implantá-la em toda a
infraestrutura e torná-la acessível a todos.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_13** – *“A practice in which code under test is first released
    to a small batch of real users. If the metrics deviate from nominal
    ranges, routing to canary release might automatically halt.”*

-   **EP\_28** – *‘Canary deployment used in Case E ensured testing in
    production environment with the users.[...] such as canary release
    that exposes software changes incrementally to a portion of users
    before deploying them to entire user base.’’*

A estratégia de implantação conhecida como ***“dark launch”*** sugeridas
nos (EP\_13, EP\_50), descreve o processo de liberar uma funcionalidade
ou recurso para um subconjunto de usuários afim de obter respostas do
usuário, sendo que esses usuários não sabem que estão sendo testados e
não têm a nova funcionalidade apontada para eles de forma alguma, por
exemplo o lançamento experimental de uma compra de um clique para meus
usuários afim de avaliar se irá ocorrer o aumento das vendas.

*Dark Launches* e Implantações Canários são bastante semelhantes, pois
ambos lidam com o lançamento de novas funcionalidades no ambiente de
produção para um subconjunto de usuários reais antes de liberar para
todos, desvinculando a implantação do lançamento. No entanto, a
Implantação Canária são mais comumente usadas para testar novos recursos
no back-end, afim de fazer a transição lentamente para uma nova
infraestrutura.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_13** – *“This dark launch lets the engineer slowly deploy and
    stabilize small chunks directly during production without impacting
    the user experience. After stabilization, the engineer can turn on
    the feature and release it.[...] Instagram often uses dark launches
    to deploy and stabilize features for up to six months before
    officially releasing them. Microsoft often deploys large
    architectural changes, using a combination of dark launches and
    feature flags.”*

-   **EP\_50** – *“dark launches: A deployment strategy where changes
    are released during off peak hours; or where code is installed on
    all servers, but configured so that users do not see their effects
    because their user interface components are switched off. Such
    launches can be used to test scalability and performance [14] and
    can be used to break a larger release into smaller ones.”*

Os autores em (EP\_28, EP\_50) sugeriram outra estratégia de implantação
chamada ***“Blue-Green Deployments”*** que é um modelo de implantação
que transfere gradualmente o tráfego de usuários de uma versão anterior
(azul) da aplicação ou microsserviço para uma nova versão (verde),
estando ambas as versões em execução em ambiente de produção idênticos,
eliminando o tempo de inatividade devido à implantação do aplicativo.
Quando o ambiente verde estiver com todo o trafego, o ambiente azul
ficará offline e poderá servir de standby como opção de recuperação de
desastres ou tornar-se o ambiente da próxima atualização.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_28** – *“The cases employed different deployment strategies,
    such as blue-green deployment (Cases C and E)[...]”*

-   **EP\_50** – *“blue-green deployments: A deployment strategy where a
    defective change to a production environment (blue) can be quickly
    switched to the latest stable production build (green) [15].”*

Diferente da *“Blue-Green Deployments”* que cria um ambiente separado
para a uma nova versão, sem afetar a antiga, onde são realizados testes
na nova versão e, uma vez pronta, inicia-se o encaminhamento dos
usuários para a nova versão. Já o ***“Rolling Upgrade”*** apresentado no
(EP\_28), possibilita que a nova versão seja implantada gradualmente nos
servidores de produção fazendo com que o *cluster* torne-se
heterogêneos, ou seja, havendo servidores com a versão antiga e outros
com a nova versão, até a nova versão ter sido implantada todos os
servidores. Essa estratégia tem como objetivo final de substituir
lentamente todas as versões antigas pelas novas.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_28** – *“The cases employed different deployment strategies,
    such as blue-green deployment (Cases C and E), rolling upgrade (Case
    B)[...]”*

A estratégia de implantação ***“Staging/Baking”*** mencionada no
(EP\_50) consiste de se ter uma etapa antes do lançamento para a
produção, como uma especie de ensaio final. Essa etapa é denomidada
*staging* ou “encenação” a qual a nova versão do software é testada
tendo com o objetivo de garantir que a aplicação atenda aos requisitos e
expectativas dos negócios, em um ambiente identico ao de produção (isso
significa que as configurações da máquina entre a encenação e a produção
devem coincidir).

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_50** – *“staging/baking: A stage in the deployment pipeline
    where a new version of software is tested in conditions similar to a
    production environment. An example of this is called shadow testing
    where production traffic is cloned and sent to a set of shadow
    machines that execute newer code than production. Results between
    production and shadow environments can be automatically compared and
    discrepancies reported as failures.”*

### MP20. Definir Mecanismo de Rollback {#mp20.-definir-mecanismo-de-rollback .unnumbered}

Quando uma nova funcionalidade gera defeitos na produção deve-se ter um
plano para reverter ao estado anterior. A adoção de uma estratégia de
reversão deve ser definida em conjunto com a de implantação, pois a essa
estratégia tende a espelhar a de implantação. Como mencionado
anteriormente algumas estratégias de implantação, como a implantação
canário, *dark launch*, implantação *blue-green* e a *rolling upgrade*,
por exemplo, possibilitam e reversão da implantação por definição.

Seguem transcrições de evidências relacionadas a esse tópico:

-   **EP\_** – *“The cases employed different deployment strategies,
    such as blue-green deployment (Cases C and E), rolling upgrade (Case
    B) and canary deployment (Case E). Roll-back mechanism was said to
    be in place in Cases B, C, D and E.”*

<span>llc</span> [tbl:praticas~p~ipeline]\

& &\

& &\
 & EP\_28, EP\_39 &\
 & EP\_39 &\
 & EP\_39 &\
 & &\
MP6. Commits pequenos & &\
 & EP\_15 &\
MP8. Refatoração & EP\_06 &\
MP9. Revisão de Código & &\
 & &\
 & EP\_06 &\
 & &\
 & EP\_06 &\
 & &\
&\
& &\
 & EP\_14, EP\_32 &\
MP16. Microsserviços & &\
MP17. Build automatizado & &\
 & EP\_28, EP\_48 &\
 & &\
 & EP\_28 &\

### Q3. Quais ferramentas foram empregadas para projetar e implementar pipelines de implantação? {#subsec:srl_rq4_ferramentas}

Esta seção apresenta as conclusões para responder a RQ2. Investigamos a
cadeia de ferramentas de implantação relatada na literatura. Foram
encontradas 61 ferramentas de apoio para adoção de pipelines de
implantação as quais foram categorizadas em 9 categorias: (i)
gerenciamento de projetos; (ii) sistema de controle de versão ou em
inglês ; (iii) ferramenta de gerenciamento e análise de código; (iv)
construir ferramenta; (v) servidor de integração contínua; (vi)
ferramenta de teste; (vii) repositório de artefatos; (viii) configuração
e provisionamento; e (ix) monitoramento.

Deve-se notar que as ferramentas relatadas nesta seção são, em sua
maioria, fontes abertas e ferramentas comerciais existentes, que visam
formar e implementar um pipeline de implantação. Essas ferramentas são
apresentadas e descritas abaixo e sumarizadas na .

**F1. Jira:** Jira é uma família de produtos criada para ajudar todos os
tipos de equipes a gerenciarem seu trabalho. A ferramenta permite o
monitoramento de tarefas e acompanhamento de projetos garantindo o
gerenciamento de todas as suas atividades em único lugar.

**F2. Atlassian Confluence:** O Confluence é o espaço de trabalho da
equipe em que o conhecimento e a colaboração andam lado a lado. Através
da criação de páginas dinâmicas para quase tudo, de planos de projeto a
anotações de reuniões, guias de solução de problemas, políticas e entre
outros, a equipe pode criar, coletar e colaborar em qualquer projeto ou
ideia. As páginas são armazenadas em espaços, espaços de trabalho em que
é possível colaborar no trabalho e manter todo o conteúdo organizado
além de compartilhar o trabalho, para que cada membro da equipe possa
ver o conhecimento institucional e acessar as informações necessárias
para realizar o melhor trabalho.

**F3. IBM Rational Team Concert (RTC):** Ferramenta de colaboração da
equipe de desenvolvimento de software, desenvolvida pela Rational
Software uma marca da IBM, que fornecer recursos que integram tarefas de
projeto de desenvolvimento, incluindo planejamento de iteração,
definição de processo, gerenciamento de mudanças, rastreamento de
defeitos, controle de versão, automação da compilação e relatório.

**F4. Git:** Sistema de controle de versões distribuído, usado
principalmente no desenvolvimento de software, mas pode ser usado para
registrar o histórico de edições de qualquer tipo de arquivo.

**F5. GitHub:** Plataforma de hospedagem de código-fonte com controle de
versão usando o Git. Ele permite que programadores, utilitários ou
qualquer usuário cadastrado na plataforma contribuam em projetos
privados e/ou Open Source de qualquer lugar do mundo.

**F6. GitLab:** Gerenciador de repositório de software baseado em Git,
com suporte a Wiki, gerenciamento de tarefas e CI/CD. GitLab é similar
ao GitHub, mas o GitLab permite que os desenvolvedores armazenem o
código em seus próprios servidores, ao invés de servidores de terceiros.

**F7. BitBucket:** Serviço de hospedagem de projetos controlados através
do Mercurial, um sistema de controle de versões distribuído. É similar
ao GitHub (que utiliza Git). Bitbucket têm um serviço grátis e um
comercial.

**F8. Apache Subversion (SVN):** Sistema de controle de versão desenhado
especificamente para ser um substituto moderno do Concurrent Version
System (CVS), que se considera ter algumas limitações. O Subversion
utiliza banco de dados Berkeley BD.

**F9. Deveo:** Deveo é uma plataforma de hospedagem e colaboração de
código que suporta repositórios Git, Subversion e Mercurial. Além da
hospedagem de código, a Deveo oferece revisões de código, rastreamento
de problemas (*issue tracking*) e recursos de documentação.

**F10. Azure DevOps:** Azure DevOps Services é um serviço de nuvem
oferecido pela Microsoft, com o objetivo de colaboração no
desenvolvimento de código. Ele provê funcionalidades integradas que você
pode acessar via web browser ou a IDE do Visual Studio. As
funcionalidades incluídas são: Boards, Repositories, Pipelines,
Artifacts e Test Plans. O Azure Repos fornece repositórios Git privados,
hospedados na nuvem e ilimitados permitindo a colaboração para compilar
códigos melhores com solicitações de pull e gerenciamento de arquivos
avançado.

**F11. SonarQube:** Plataforma de código aberto desenvolvida pela
SonarSource para inspeção contínua da qualidade do código para realizar
revisões automáticas com análise estática de código para detectar bugs,
cheiros de código e vulnerabilidades de segurança em mais de 20
linguagens de programação. O SonarQube oferece relatórios sobre código
duplicado, padrões de codificação, testes unitários, cobertura de
código, complexidade de código, comentários, bugs e vulnerabilidades de
segurança.

**F12. Microsoft Baseline Security Analyzer:** Ferramenta de software
descontinuada que não está mais disponível na Microsoft que determina o
estado de segurança, avaliando atualizações de segurança ausentes e
configurações de segurança menos seguras dentro do Microsoft Windows,
componentes do Windows, como o Internet Explorer, o servidor web IIS e
os produtos Microsoft SQL Server e as configurações de macro do
Microsoft Office.

**F13. Attack Surface Analyzer:** Ferramenta criada para a análise de
alterações feitas na superfície de ataque dos sistemas operacionais
desde o Windows Vista, ajudando a identificar potenciais riscos de
segurança introduzidos por um software novo ou não confiável, detectando
alterações nas áreas-chave da configuração de segurança do sistema.

**F14. CodeSonar:** Principal software de análise estática de teste de
segurança de aplicativo estático (SAST) da GrammaTech, que identifica
erros que podem resultar em falhas no sistema, comportamentos
inesperados e violações de segurança.

**F15. Klocwork:** Ferramenta de análise de código estático para C, C++,
C\#e Java de propriedade do desenvolvedor de software Perforce, que
identifica problemas de segurança, qualidade e confiabilidade do
software que ajudam a impor a conformidade com as normas de segurança.

**F16. Gerrit:** Software livre para revisão de códigos fonte no
processo de desenvolvimento de softwares com auxilio do navegador de
internet para projetos que fazem controle de versão com o Git, onde os
desenvolvedores autorizados enviam alterações podem ser aprovar ou
reprovar automaticamente, exibindo as alterações lado a lado no
navegador e permite comentários in-line.

**F17. Gradle:** Sistema de automação de compilação open source que se
baseia nos conceitos de Apache Ant e Apache Maven e introduz uma
linguagem de domínio específico (DSL) baseada em Groovy em vez do XML
usado pelo Apache Maven para declarar a configuração do projeto.

**F18. Apache Maven:** Ferramenta de automação de compilação,
gerenciamento e compreensão de projetos de software utilizada
primariamente em projetos Java. Com base no conceito de um modelo de
objeto de projeto (POM), a Maven pode gerenciar a compilação, relatórios
e documentação de um projeto a partir de uma informação central.

**F19. Apache Ant:** Biblioteca Java e ferramenta de linha de comando
cuja missão é conduzir processos descritos em arquivos de construção
como alvos e pontos de extensão dependentes uns dos outros. O principal
uso conhecido do Ant é a construção de aplicações Java. A Ant fornece
uma série de tarefas incorporadas que permitem compilar, montar, testar
e executar aplicativos Java.

**F20. Jenkins:** Servidor de automação de código aberto e livre. Ajuda
a automatizar as partes do desenvolvimento de software relacionadas à
construção, testee implantação, facilitando a integração contínua e a
entrega contínua.

**F21. Travis CI:** Serviço de integração contínua hospedado usado para
construir e testar projetos de software hospedados no GitHub e
bitbucket, fornecendo vários planos pagos para projetos privados, e um
plano gratuito para código aberto.

**F22. GoCD:** Ferramenta de código aberto que é usada no
desenvolvimento de software para ajudar equipes e organizações a
automatizar a entrega contínua (CD) do software. Ele suporta automatizar
todo o processo de liberação de teste de compilação desde o check-in de
código até a implantação.

**F23. GitLab CI/CD:** Ferramenta poderosa incorporada ao GitLab que
permite aplicar todos os métodos contínuos (Integração Contínua, Entrega
e Implantação) ao seu software sem necessidade de aplicação ou
integração de terceiros.

**F24. Bamboo CI:** Servidor de integração contínua (CI) da Atlassian
que pode ser usado para automatizar o gerenciamento de lançamentos para
um aplicativo de software, criando um pipeline de entrega contínua.

**F25. TeamCity:** Servidor de gerenciamento de construção e integração
contínua da JetBrains, sendo um software comercial e licenciado sob uma
licença proprietária e possui uma licença gratis para até 100
configurações de construção e três agentes de construção que podem ser
executados simultaneamente.

**F26. Circle CI:** Plataforma DE CI/CD permite que as equipes liberem
rapidamente o código em que confiam, automatizando o processo de
construção, teste e entrega para aplicativos móveis e web, tanto na
nuvem quanto em seu próprio servidor privado.

**F27. AppVeyor:** Serviço de integração contínua hospedado e
distribuído usado para construir e testar projetos hospedados no GitHub
e outros serviços de hospedagem de código-fonte (incluindo GitLab e
Bitbucket) em uma máquina virtual Microsoft Windows ou Linux.

**F28. CloudBees:** Provedor de serviços de software de entrega
contínua, que permite que as organizações construam, testem e implantem
aplicativos para produção, utilizando práticas contínuas de entrega. A
família de produtos CloudBees inclui uma versão corporativa do Jenkins,
fornecendo suporte comercial e plugins adicionais para jenkins de código
aberto. A Plataforma CloudBees Jenkins inclui o CloudBees Jenkins
Operations Center, que fornece uma maneira central de gerenciar Jenkins
em uma organização. As versões masters e plugin são mais facilmente
mantidas e os recursos podem ser compartilhados entre as equipes
jenkins.

**F29. Wercker:** Plataforma de entrega contínua baseada no Docker que
ajuda os desenvolvedores de software a construir e implantar seus
aplicativos e microsserviços.

**F30. Azure DevOps:** O Azure Pipelines é um serviço em nuvem que
integra o pacote de serviços Azure DevOps e que você pode ser usado para
construir e testar automaticamente seu projeto de código e
disponibilizá-lo para outros usuários. Ele funciona com quase qualquer
linguagem de programação ou tipo de projeto. O Azure Pipelines combina a
integração contínua (CI) e a entrega contínua (CD) para testar e
construir seu código de forma constante e consistente para qualquer
alvo.

**F31. IBM Rational Quality Manager (RQM):** Solução de gerenciamento de
testes parte do IBM Rational CLM (*Collaborative Life Cycle Management*)
que ajuda o usuário com atividades de gerenciamento de qualidade, como
Planejamento de Testes, Criação de Casos de Teste, Execução de Casos de
Teste e Relatórios de Testes.

**F32. Apache JMeter:** Software de código aberto, um aplicativo Java
100% puro projetado para carregar o comportamento funcional do teste e
medir o desempenho. Foi originalmente projetado para testar aplicações
web, mas desde então expandiu-se para outras funções de teste. O Apache
JMeter pode ser usado para testar o desempenho tanto em recursos
estáticos quanto dinâmicos, aplicações dinâmicas da Web. Ele pode ser
usado para simular uma carga pesada em um servidor, grupo de servidores,
rede ou objeto para testar sua força ou para analisar o desempenho geral
em diferentes tipos de carga.

**F33. Gatling:** Framework de teste de carga e desempenho de código
aberto baseada em Scala, Akka e Netty. O Gatling foi projetado para ser
usado como uma ferramenta de teste de carga para analisar e medir o
desempenho de uma variedade de serviços, com foco em aplicações web.

**F34. Cucumber:** Ferramenta de software que suporta BDD
(*Behavior-Driven Development*, desenvolvimento orientado pelo
comportamento. A ab abordagem central do Cucumber BDD é o seu analisador
de linguagem natural chamado Gherkin. Ele permite que os comportamentos
de software esperados sejam especificados em uma linguagem lógica que os
clientes possam entender. Como tal, o Cucumber permite a execução da
documentação de recursos escrita em texto voltado para os negócios.

**F35. Fortify:** Provedor de segurança de aplicativos que oferece
testes estáticos de segurança de aplicativos (SAST), testes dinâmicos de
segurança de aplicativos (DAST), teste interativo de segurança de
aplicativos (IAST) e autoproteção de aplicativos de tempo de execução
(RASP) no local e sob demanda.

**F36. Selenium:** Conjunto de ferramentas de código aberto
multiplataforma, usado para testar aplicações web pelo navegador
(*browser*) de forma automatizada. Ele executa testes de funcionalidades
da aplicação web e testes de compatibilidade entre *browser* e
plataformas diferentes. O Selenium suporta diversas linguagens de
programação, como por exemplo C\#, Java e Python, e vários navegadores
web como o Chrome e o Firefox.

**F37. Smokemonster:** O EP\_49 informa que em 2015 os ambientes dos
clientes da empresa a qual foi realizado o estudo de caso eram
realizados *smoke test* (teste de fumaça) através do Smokemonster.

**F38. Nexus Repository Manager:** Gerente de repositório que permite
armazenar e recuperar artefatos de construção. Assim, a empresa pode
hospedar seus próprios repositórios, mas também usar o Nexus como um
proxy para repositórios públicos. Com tal proxy o tempo para receber um
artefato é reduzido e economiza largura de banda. Nexus permite que você
hospede seus artefatos de construção privada. O Nexus está disponível
como distribuição comercial e *open source*.

**F39. JFrog Artifactory:** Gerenciador de repositórios para empresas
que suporta todos os tipos de pacotes de software disponíveis, com
suporte seguro, agrupado e de alta disponibilidade para registros
Docker, integrando-se com todas as principais ferramentas de / e ,
fornecendo uma solução automatizada e forte para rastrear artefatos do
desenvolvimento à produção.

**F40. Ansible:** Ferramenta de TI de código aberto para gerenciar,
automatizar, configurar servidores (tipo Unix e Microsoft Windows) e,
implantar aplicativos, a partir de uma localização central (normalmente
de um sistema Unix).

**F41. Plataforma System Center Orchestrator:** Solução de gerenciamento
de fluxo de trabalho para data centers. Com o System
Center-Orchestrator, pode-se unir tarefas e procedimentos diferentes
usando uma interface gráfica do usuário Runbook Designer para criar
soluções de ponta a ponta confiáveis, flexíveis e eficientes no ambiente
de ti. Usando o Orchestrator, pode-se: (i) automatizar processos do data
center, independentemente do hardware ou plataforma; (ii) padronizar
práticas recomendadas para melhorar a eficiência operacional; (iii)
conectar sistemas de fornecedores diferentes sem precisar saber como
usar scripts e linguagens de programação.

**F42. AWS Cloud:** A Amazon Web Services (AWS) é a plataforma de nuvem
mais adotada e mais abrangente do mundo, oferecendo mais de 175 serviços
completos de datacenters em todo o mundo: de tecnologias de
infraestrutura, como computação, armazenamento e bancos de dados, a
tecnologias emergentes como machine learning e inteligência artificial,
data lakes, análises e Internet das Coisas.

**F43. Vagrant:** Software de código aberto para criar e manter
ambientes de desenvolvimento virtuais portáteis, utilizando VirtualBox,
KVM, Hyper-V, Docker containers, VMware, e AWS. Ele tenta simplificar a
gerência de configuração de software das virtualizações para aumentar a
produtividade do desenvolvimento.

**F44. Puppet:** Ferramenta de automação de servidor de código aberto. É
composto por uma linguagem declarativa para expressar a configuração do
sistema, um cliente e um servidor para distribuí-lo e uma biblioteca
para realizar a configuração.

**F45. SSH:** Acrônimo de Secure Shell, é um protocolo de rede
criptográfico para operação de serviços de rede de forma segura sobre
uma rede insegura. No survey realizado no EP\_23, foi constatado que 50%
dos profissionais usavam SSH como um sistema de implantação.

**F46. Nolio:** Ferramenta de implantação de aplicativos que regula e
acelera a entrega de aplicativos em toda a empresa, permitindo
implantações de toque zero desde o desenvolvimento até a produção.

**F47. Chef:** Ferramenta de gerenciamento de configuração, que usa uma
linguagem pura-ruby, específica de domínio (DSL) para escrever
“receitas” de configuração do sistema. O Chef é usado para agilizar a
tarefa de configurar e manter os servidores de uma empresa, e pode se
integrar a plataformas baseadas em nuvem.

**F48. Docker:** Conjunto de produtos de plataforma como serviço (PaaS)
que usam virtualização de nível de sistema operacional para entregar
software em pacotes chamados contêineres. Um contêiner é uma unidade
padrão de software que embala código e todas as suas dependências para
que o aplicativo seja executado de forma rápida e confiável de um
ambiente de computação para outro. Uma imagem de contêiner Docker é um
pacote leve, autônomo e executável de software que inclui tudo o que é
necessário para executar um aplicativo: código, tempo de execução,
ferramentas do sistema, bibliotecas e configurações do sistema. Os
contêineres são isolados uns dos outros e agrupam seus próprios
softwares, bibliotecas e arquivos de configuração. Eles podem se
comunicar uns com os outros por meio de canais bem definidos. Todos os
contêineres são executados por um único kernel do sistema operacional e,
portanto, usam menos recursos do que as máquinas virtuais.

**F49. Kubernetes (K8s):** Sistema de orquestração de contêineres
open-source que automatiza a implantação, o dimensionamento e a gestão
de aplicações em contêineres.

**F50. Chake:** Ferramenta que ajuda você a gerenciar vários hosts sem a
necessidade de um chef server. A configuração é gerenciada em um
diretório local, que provavelmente deve estar sob controle de versão com
git ou qualquer outro. A configuração geralmente é implantada via rsync
sobre SSH e aplicada invocando chef-solo sobre SSH em cada host.

**F51. Nagios:** Aplicação de monitoramento de rede de código aberto
distribuída sob a licença GPL permitindo o monitoramento de todos os
componentes de infraestrutura de missão crítica, incluindo aplicativos,
serviços, sistemas operacionais, protocolos de rede, métricas de
sistemas e infraestrutura de rede.

**F52. CA Service Ope-rations Insight (SOI):** Software de gerenciamento
de serviço para auxiliar os usuários em e engenharia a gerenciar a
qualidade e a disponibilidade de serviços online, unificando as
informações de saúde e disponibilidade da ferramentas de gerenciamento
de domínio e alinhando-se com os serviços de TI. É um sistema de gestão
de relacionamento com o cliente que orienta na tomada de ações
específicas e adequadas às prioridades do negócio.

**F53. Apache Kafka:** Plataforma *open source* de processamento de
streams desenvolvida pela Apache Software Foundation que tem como
objetivo fornecer uma plataforma unificada, de alta capacidade e baixa
latência para tratamento de dados em tempo real.

**F54. Linux Tracing Toolkit Next Generation (LTTng):** Estrutura de
rastreamento de código aberto para Linux, foi projetado para um impacto
mínimo de desempenho e tendo um impacto próximo de zero quando não é
rastreamento, é útil para depurar uma ampla gama de bugs que são
extremamente desafiadores.

**F55. Dynatrace:** Plataforma de inteligência de software baseada em
inteligência artificial para fornecer monitoramento de desempenho de
aplicativos (APM), inteligência artificial para operações (AIOps),
monitoramento de infraestruturade TI, gerenciamento de experiência
digital (DEM) e recursos de análise de negócios digitais.

**F56. New Relic:** Ferramenta de monitoramento e aperfeiçoamento de
recursos e aplicativos em servidores.

**F57. System:** No survey realizado no EP\_23 os autores descobriram
que para monitorar o desempenho, os profissionais tendem a confiar em
ferramentas de sistema de nível inferior.

**F58. GrayLog:** Ferramenta *open source* utilizado para centralização,
ordenar e classificar os logs em forma de index afim de analisar os logs
de sua infraestrutura de maneira eficiente, direcionando assim todos os
logs dos diversos ativos para um único host, facilitando uma auditoria e
a identificação de algum problema.

**F59. AWS Monitoring Services:** O Amazon CloudWatch é um serviço de
monitoramento e observação criado para engenheiros de DevOps,
desenvolvedores, Site Reliability Engineers (SREs – Engenheiros de
confiabilidade de sites) e gerentes de TI.

**F60. Amazon Kinesis:** Serviço que facilita a coleta, o processamento
e a análise de dados de streaming em tempo real, permitindo que você
obtenha insights oportunos e reaja rapidamente às novas informações.

**F61. Dataloop.io:** Serviço de monitoramento para equipes de DevOps e
Operações que executam implantações de nuvem, SaaS, microsserviços e
IoT.

<span>lllc</span> [tbl:ferramentas~p~ipeline]\

& & &\

& F1. Jira & EP\_12 &\
 & & EP\_15 &\
 & & EP\_05 &\

& F4. Git & &\
 & F5. GitHub & &\
 & F6. GitLab & &\
 & F7. BitBucket & EP\_12, EP\_28 &\
 & & EP\_23 &\
 & F9. Deveo & EP\_28 &\
 & F10. Azure DevOps & EP\_35 &\

& F11. SonarQube & &\
 & & EP\_10 &\
 & & EP\_10 &\
 & F14. CodeSonar & EP\_12 &\
 & F15. Klocwork & EP\_12 &\
 & F16. Gerrit & EP\_31 &\

& F17. Gradle & EP\_04, EP\_06 &\
 & F18. Maven & &\
 & F19. Ant & EP\_06 &\

& F20. Jenkins & &\
 & F21. Travis CI & &\
 & F22. GoCD & EP\_09 &\
 & F23. GitLab CI/CD & EP\_11, EP\_39 &\
 & F24. Bamboo CI & EP\_12 &\
 & F25. TeamCity & EP\_15 &\
 & F26. CircleCI & EP\_22, EP\_34, EP\_36 &\
 & F27. AppVeyor & EP\_22 &\
 & F28. CloudBees & EP\_22 &\
 & F29. Wercker & EP\_22 &\
 & F30. Azure DevOps & EP\_35 &\

& & EP\_05 &\
 & F32. JMeter & EP\_10 &\
 & F33. Gatling & EP\_15 &\
 & F34. Cucumber & EP\_15 &\
 & F35. Fortify & EP\_24 &\
 & F36. Selenium & EP\_28 &\
 & F37. Smokemonster & EP\_49 &\

& F38. Nexus & EP\_02 &\
 & F39. Artifactory & EP\_06, EP\_24 &\

& F40. Ansible & EP\_02, EP\_28, EP\_49 &\
 & & EP\_05 &\
 & F42. AWS Cloud & &\
 & F43. Vagrant & EP\_12, EP\_28, EP\_49 &\
 & F44. Puppet & &\
 & F45. SSH (deploy) & EP\_23 &\
 & F46. Nolio & EP\_24 &\
 & F47. Chef & &\
 & F48. Docker & &\
 & F49. Kubernetes & EP\_35 &\
 & F50. Chake & EP\_38 &\

& F51. Nagios & EP\_02, EP\_23 &\
 & & EP\_05 &\
 & F53. Apache Kafka & EP\_06 &\
 & & EP\_12 &\
 & F55. Dynatrace & EP\_23 &\
 & F56. New Relic & EP\_23, EP\_28 &\
 & F57. System & EP\_23 &\
 & F58. GrayLog & EP\_28 &\
 & & EP\_28 &\
 & F60. Kinesis & EP\_28 &\
 & F61. Dataloop.io & EP\_49 &\

