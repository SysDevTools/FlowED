# Linha do Tempo da Develop

## Visão Geral

A branch `develop` é o principal espaço de trabalho para o desenvolvimento contínuo no `FlowED`. Ela é usada para integrar todas as novas funcionalidades e melhorias antes que sejam preparadas para lançamento. Esta linha do tempo reflete o estado atual do desenvolvimento e serve como base para a criação de releases.

## Ciclo de Vida

1. **Criação de Feature Branches:**
   - Novas funcionalidades e correções são desenvolvidas em branches separadas a partir da `develop`.
   - Essas feature branches são integradas de volta na `develop` após passarem por revisões e testes.

2. **Integração Contínua:**
   - A `develop` é constantemente atualizada com novas integrações, refletindo o progresso do desenvolvimento.
   - Essa branch nunca é usada para deploy em produção diretamente; é uma área de preparação e testes.

3. **Transição para Release:**
   - Quando a `develop` atinge um estado de estabilidade com um conjunto coeso de funcionalidades, uma branch `release` é criada a partir dela.
   - A `develop` continua a ser usada para novos desenvolvimentos enquanto a `release` segue para homologação e publicação.

## Referências

- Veja mais detalhes sobre o ciclo de desenvolvimento no [documento de ciclos](./docs/pt-br/cycles/development.md).
- Consulte as [Níveis de Implementação](./docs/pt-br/levels/intermediate.md) para entender como a `develop` é usada em diferen
