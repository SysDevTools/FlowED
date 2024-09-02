# Linha do Tempo das Releases

## Visão Geral

As branches `release` são temporárias e servem para estabilizar uma versão específica antes de sua publicação. Elas são derivadas da `develop` e, uma vez aprovadas, são integradas na `main`.

## Ciclo de Vida

1. **Criação da Release:**
   - Uma branch `release` é criada a partir da `develop` quando um conjunto de funcionalidades é considerado pronto para estabilização.
   - Essa branch é usada para correções finais e ajustes menores necessários para preparar a versão para produção.

2. **Estabilização e Testes:**
   - A `release` passa por testes rigorosos, incluindo testes de integração e aceitação por stakeholders.
   - Apenas correções críticas são permitidas durante esta fase, evitando a introdução de novas funcionalidades.

3. **Finalização e Integração:**
   - Após a aprovação final, a branch `release` é integrada na `main` para publicação e na `develop` para manter a consistência.
   - A branch `release` é então deletada, tendo cumprido seu propósito.

## Referências

- Para mais informações sobre o ciclo de homologação, consulte o [documento de ciclos](./docs/pt-br/cycles/homologation.md).
- As releases são uma parte crítica dos [Níveis de Implementação](./docs/pt-br/levels/intermediate.md).
