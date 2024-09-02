# Linha do Tempo da Main

## Visão Geral

A branch `main` representa o histórico oficial de releases do projeto. Ela contém apenas o código que foi aprovado e publicado, refletindo as versões estáveis que estão ou estiveram em produção.

## Ciclo de Vida

1. **Integração de Releases:**
   - Novas releases aprovadas são integradas à `main`, marcando a transição de uma versão para a produção.
   - Apenas código que passou por todo o ciclo de homologação e foi considerado estável é integrado na `main`.

2. **Deploy em Produção:**
   - A `main` é usada para deploy em produção. Cada commit nela representa uma versão do software que foi ou será entregue aos usuários finais.

3. **Gestão de Hotfixes:**
   - Se problemas críticos são encontrados após o deploy, eles são resolvidos em branches `hotfix` criadas a partir da `main`.
   - Após correções, os hotfixes são integrados de volta na `main` e propagados para `develop` e `release`.

## Referências

- Para mais detalhes sobre o ciclo de publicação, consulte o [documento de ciclos](./docs/pt-br/cycles/publication.md).
- A `main` é parte central de todos os [Níveis de Implementação](./docs/pt-br/levels/advanced.md).
