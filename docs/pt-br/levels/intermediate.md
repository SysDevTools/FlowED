# Nível 2: Implementação Intermediária

## Visão Geral

O Nível 2 do `FlowED` é ideal para pequenas equipes ou projetos que, embora comecem simples, exigem mais controle e organização à medida que crescem. Esse nível introduz a separação entre as linhas do tempo de desenvolvimento e release, permitindo maior granularidade e controle no fluxo de trabalho. Ele é adequado para equipes que precisam de mais estrutura, mas ainda assim prezam pela simplicidade.

## Estrutura do Nível 2

- **Duas Linhas do Tempo:**
  - **Linha do Tempo de Desenvolvimento (`develop`):** Onde todo o trabalho de desenvolvimento acontece. Inclui commits frequentes e pode envolver múltiplos desenvolvedores.
  - **Linha do Tempo de Release (`release`):** Um ramo intermediário que consolida as mudanças significativas antes de serem promovidas para a `main`.

- **Branches Principais:**
  - **Develop:** Branch para o desenvolvimento contínuo. Aqui é onde todas as features e correções são integradas.
  - **Release:** Branch usada para preparar a próxima versão. Permite a integração de várias features e a estabilização do código antes da publicação.
  - **Main:** Branch de produção, onde as versões estáveis e publicadas do software residem.

## Ciclo de Ações

1. **Inicialização do Repositório:**
   - Crie um repositório no GitHub, configurando as branches `develop` e `release`, além da `main`.
   - Clone o repositório e configure o ambiente local para suportar a estrutura de branches.

2. **Desenvolvimento Contínuo na Branch `Develop`:**
   - Os desenvolvedores trabalham na branch `develop`, realizando commits frequentes.
   - Toda nova feature ou correção é integrada nesta branch, garantindo que o desenvolvimento seja contínuo e colaborativo.

3. **Criação e Preparação do Release:**
   - Quando o desenvolvimento atinge um ponto de estabilidade ou preparação para uma nova versão, cria-se uma branch `release` a partir da `develop`.
   - Essa branch serve para integrar e estabilizar as mudanças antes da publicação.
   - Correções de bugs menores e ajustes finais são feitos na `release`, sem impactar diretamente a `develop`.

4. **Homologação e Feedback:**
   - A branch `release` passa por testes de homologação e feedback de stakeholders.
   - Correções feitas durante a homologação são integradas na `release`, garantindo que a versão está estável antes de ser promovida.

5. **Merge e Publicação na `Main`:**
   - Após a homologação, a `release` é integrada na `main`.
   - A `main` é atualizada e a versão é publicada com um novo número de versão seguindo o versionamento semântico.
   - A branch `release` também é integrada de volta na `develop`, garantindo que as mudanças sejam refletidas no desenvolvimento contínuo.

6. **Criação de Novo Release:**
   - Com a `main` atualizada, um novo ciclo de desenvolvimento pode começar na `develop`.
   - O próximo release segue o mesmo processo, garantindo uma iteração contínua.

## Exemplos de Uso

- **Pequenos Projetos em Equipe:**
  - Projetos de software que envolvem uma pequena equipe podem se beneficiar da estrutura mais organizada e da separação entre desenvolvimento e release.
  - Cada membro da equipe pode trabalhar em features diferentes na `develop`, enquanto a `release` serve como um buffer para integração e estabilização antes da publicação.

- **Projetos em Crescimento:**
  - Projetos que começaram simples, mas começaram a crescer em escopo e complexidade, podem adotar esse nível para manter a organização sem perder a simplicidade do `FlowED`.

## Vantagens do Nível 2

- **Organização Melhorada:** A separação entre `develop` e `release` permite maior controle e menos riscos ao integrar novas mudanças.
- **Homologação Efetiva:** A branch `release` oferece um espaço dedicado para testes e homologação antes da publicação.
- **Colaboração Facilitada:** Com uma estrutura clara de branches, equipes podem colaborar de forma mais eficiente, sem pisar no trabalho um do outro.

## Ferramentas Recomendadas

- **GitHub:** Para controle de versão e repositório remoto.
- **CI/CD (ex: GitHub Actions):** Automatize testes e integrações na branch `release` para garantir estabilidade.
- **Editor de Código (VSCode, JetBrains):** Suporte integrado para Git e CI/CD.
