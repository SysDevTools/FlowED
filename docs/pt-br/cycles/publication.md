# Ciclo de Publicação

## Visão Geral

O Ciclo de Publicação no `FlowED` cobre as etapas finais de entrega de software. Este ciclo é dedicado à integração final, publicação na branch `main` e realização de ajustes emergenciais através de hotfixes.

## Etapas do Ciclo de Publicação

1. **Integração na Main:**
   - Após a aprovação na homologação, a branch `release` é integrada na `main`.
   - Este merge finaliza o ciclo de desenvolvimento, publicando a versão estável do software.

2. **Deploy em Produção:**
   - A versão publicada na `main` é implantada no ambiente de produção.
   - Testes de smoke são realizados para garantir que a implantação foi bem-sucedida e que a aplicação está funcionando corretamente.

3. **Gestão de Hotfixes:**
   - Caso sejam identificados problemas críticos após a publicação, uma branch `hotfix` é criada a partir da `main`.
   - O `hotfix` é implementado rapidamente e integrado de volta na `main`, `develop` e, se necessário, na `release`.
