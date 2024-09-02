# `FlowED` (Flow Education-Driven)

**FlowEd** (Flow Education-Driven - Fluxo Orientado para a Educação) é uma filosofia de gestão de projetos de software. 

Projetado para ambientes educacionais, desenvolvedores individuais e até equipes pequenas e médias, é adaptável a diferentes níveis de complexidade. 

O `FlowEd` procura simplificar e automatizar a gestão de projetos, tornando a burocracia quase transparente para o desenvolvedor.

O nome condiz com o seu principal objetivo: Educar equipes de desenvolvimento no uso de processos de engenharia de software.

## Missão

É missão deste projeto (do qual sua ajuda é bem-vinda para contribuir) oferecer uma plataforma que proporcione documentação, rastreabilidade e monitoramento, garantindo um desenvolvimento eficiente, normatizado e alinhado com as melhores práticas de engenharia. Seja para projetos simples ou para aqueles que se tornam complexos ao longo do tempo, o `FlowEd` busca atender às necessidades dos desenvolvedores, facilitando a adoção de processos estruturados sem comprometer a agilidade e a simplicidade.

## Logotipo

<div style="text-align: center;padding-top: 30px">

   ![logo](./assets/FlowED.svg)  

</div>

## Estrutura de Pastas do Projeto

<pre style="line-height: 1.2; font-size: 12px;">
📦 FlowED/
├── 📂 assets/
│   └── 📜 <a href="#logotipo">FlowED.svg</a>
├── 📂 <a href="#documentação-detalhada-e-estruturada">docs/</a>
│   └── 📂 <a href="#documentação-detalhada-e-estruturada">pt-br/</a>
│       ├── 📂 <a href="#ciclos-de-desenvolvimento">cycles/</a>
│       │   ├── 📜 <a href="./docs/pt-br/cycles/development.md">development.md</a>
│       │   ├── 📜 <a href="./docs/pt-br/cycles/homologation.md">homologation.md</a>
│       │   └── 📜 <a href="./docs/pt-br/cycles/publication.md">publication.md</a>
│       ├── 📂 <a href="#níveis-de-implementação">levels/</a>
│       │   ├── 📜 <a href="./docs/pt-br/levels/advanced.md">advanced.md</a>
│       │   ├── 📜 <a href="./docs/pt-br/levels/intermediate.md">intermediate.md</a>
│       │   └── 📜 <a href="./docs/pt-br/levels/simple.md">simple.md</a>
│       ├── 📂 <a href="#fundamentação-e-detalhamento">philosophy/</a>
│       │   ├── 📜 <a href="./docs/pt-br/philosophy/comparison-scrum.md">comparison-scrum.md</a>
│       │   ├── 📜 <a href="./docs/pt-br/philosophy/dec-b-alignment.md">dec-b-alignment.md</a>
│       │   └── 📜 <a href="./docs/pt-br/philosophy/overview.md">overview.md</a>
│       ├── 📂 <a href="#linhas-do-tempo">timelines/</a>
│       │   ├── 📜 <a href="./docs/pt-br/timelines/develop.md">develop.md</a>
│       │   ├── 📜 <a href="./docs/pt-br/timelines/main.md">main.md</a>
│       │   ├── 📜 <a href="./docs/pt-br/timelines/releases.md">releases.md</a>
│       │   └── 📜 <a href="./docs/pt-br/timelines/user-releases.md">user-releases.md</a>
│       └── 📜 <a href="./docs/pt-br/contrib-guide.md">contrib-guide.md</a>
├── 📜 <a href="./.gitignore">.gitignore</a>
├── 📜 <a href="./LICENSE">LICENSE</a>
└── 📜 <a href="./README.md">README.md</a>
</pre>

## Filosofia do FlowED

A filosofia do `FlowED` é baseada em três pilares fundamentais:

1. **Padronização e Simplicidade:**
   O `FlowED` oferece um fluxo de trabalho claro, padronizado e simplificado. Seu objetivo é facilitar a entrada de novos desenvolvedores e manter um padrão consistente de qualidade e documentação, adaptando-se rapidamente a diferentes cenários e equipes de diversos níveis de experiência. Ele é ideal tanto para projetos em andamento quanto para novos projetos que exigem uma curva de aprendizado rápida.

2. **Granularidade e Automação:**
   O `FlowED` promove a granularidade nos commits e o uso de branches desacopladas para diferentes fases de desenvolvimento, documentação e monitoramento. Isso permite que todos os commits sejam preservados, enquanto cada branch tem um nível específico de detalhe para diferentes finalidades. O [Dec-B](https://github.com/SysDevTools/Dec-B), criado para complementar o `FlowED`, gerencia não só o versionamento de código em si como também a infraestrutura, utilizando práticas de IAC (Infrastructure as Code) para automatizar a todo o ciclo de desenvolvimento e operações, sendo uma implementação dos principais processos de DevOps.

3. **Progressividade e Flexibilidade:**
   O `FlowED` define claramente as ações necessárias, mas oferece flexibilidade na escolha das ferramentas e na implementação das estratégias. Ele suporta desde projetos simples com um único desenvolvedor até equipes que trabalham em múltiplas features e releases, com diferentes cenários de infraestrutura, tanto local quanto remota.

### Fundamentação e Detalhamento

A fundamentação do `FlowED` é útil para entender como ele foi construído e em que bases ele se apoia. Abaixo, você encontrará comparações com metodologias consagradas e o alinhamento com ferramentas como o `Dec-B` (feita para este projeto), que complementam e potencializam a aplicação desta filosofia.

[Neste documento](./docs/pt-br/philosophy/overview.md) você pode encontrar fundamentos, referências e detalhamento sobre a filosofia do `FlowED`, incluindo como ela se diferencia e se inspira em metodologias consagradas como Scrum, FDD, ASD e TDD.

- **[Comparação com Scrum e outras metodologias](./docs/pt-br/philosophy/comparison-scrum.md)**: O `FlowED` compartilha várias características com o Scrum, especialmente na sua ênfase na colaboração e na iteração contínua. No entanto, o `FlowED` se diferencia ao oferecer uma abordagem mais flexível e progressiva, que pode ser adaptada a diferentes níveis de complexidade e tamanhos de equipe. Enquanto o Scrum é altamente estruturado e prescritivo, o `FlowED` permite maior flexibilidade na escolha de ferramentas e métodos, facilitando a adoção em ambientes educacionais e em projetos menores ou com equipes inexperientes.

- **[Alinhamento com Dec-B](./docs/pt-br/philosophy/dec-b-alignment.md)**: O [Dec-B](https://github.com/SysDevTools/Dec-B) é uma ferramenta essencial para a implementação do `FlowED`, especialmente em relação ao versionamento de código e de infraestrutura. Ele automatiza os comandos Git, alinhando-os com os ciclos de desenvolvimento e publicação do `FlowED`. O [Dec-B](https://github.com/SysDevTools/Dec-B) facilita a granularidade dos commits e o uso de branches desacopladas, conforme defendido pelo `FlowED`, garantindo que cada fase do desenvolvimento seja registrada e documentada adequadamente, sem sobrecarregar o desenvolvedor com tarefas manuais repetitivas. Com o [Dec-B](https://github.com/SysDevTools/Dec-B), a filosofia do `FlowED` pode ser implementada de maneira mais eficaz e eficiente, assegurando que a rastreabilidade e a qualidade sejam mantidas ao longo de todo o ciclo de vida do projeto.

## Objetivos do FlowED

A partir destes pilares, o `FlowED` tem como objetivos:

1. Facilitar a entrada e a saída de desenvolvedores.
2. Garantir a qualidade e a rastreabilidade do código.
3. Promover a eficiência e a colaboração.
4. Simplificar a gestão de projetos sem comprometer a qualidade.
5. Adaptar-se a diferentes níveis de complexidade de forma progressiva.
6. Educar, condicionar e facilitar o uso de desenvolvimento documentado e padronizado.
7. Ser uma porta de entrada para princípios e filosofias ágeis como XP e DevOps.

## Níveis de Implementação

O `FlowED` é flexível e adaptável a diferentes níveis de complexidade nos projetos, permitindo que equipes escolham o nível mais adequado para suas necessidades.

1. **Nível 1: Implementação Simples**
   - Ideal para desenvolvedores individuais ou projetos muito pequenos.
   - Utiliza uma única linha do tempo local e remota.
   - [Detalhes do Nível 1](./docs/pt-br/levels/simple.md)

2. **Nível 2: Implementação Intermediária**
   - Adequado para pequenas equipes ou projetos que começam simples e se tornam mais complexos.
   - Inclui uma linha do tempo de release, permitindo maior granularidade no controle de versões.
   - [Detalhes do Nível 2](./docs/pt-br/levels/intermediate.md)

3. **Nível 3: Implementação Avançada**
   - Para equipes que trabalham em múltiplas features e releases simultâneas.
   - Requer coordenação entre várias linhas do tempo e branches desacopladas.
   - [Detalhes do Nível 3](./docs/pt-br/levels/advanced.md)

## Linhas do Tempo

O `FlowED` adota uma abordagem de múltiplas linhas do tempo desacopladas para gerenciar o desenvolvimento e a evolução do software.

- **[Linha do Tempo da Main](./docs/pt-br/timelines/main.md)**
- **[Linha do Tempo da Develop](./docs/pt-br/timelines/develop.md)**
- **[Linhas do Tempo das Releases](./docs/pt-br/timelines/releases.md)**

## Ciclos de Desenvolvimento

O desenvolvimento no `FlowED` é organizado em ciclos claros, cada um com objetivos específicos e etapas bem definidas.

- **[Ciclo de Desenvolvimento](./docs/pt-br/cycles/development.md)**
- **[Ciclo de Homologação](./docs/pt-br/cycles/homologation.md)**
- **[Ciclo de Publicação](./docs/pt-br/cycles/publication.md)**

## Contribuição

Para contribuir com o projeto `FlowED`, siga estas etapas:

1. Crie um fork do repositório.
2. Clone o seu fork para sua máquina local.
3. Crie uma branch para a sua contribuição.
4. Faça as alterações necessárias e commit.
5. Envie suas alterações para o seu fork.
6. Crie um Pull Request descrevendo suas alterações.

Para mais detalhes sobre como contribuir, consulte o [Guia de Contribuição](./docs/pt-br/guide.md).

---

## Contato

Para dúvidas ou sugestões, entre em contato através do email: contato@flowed.org

---

## Licença

Este projeto está licenciado sob a Licença MIT. Consulte o arquivo [LICENSE](./LICENSE) para mais detalhes.
