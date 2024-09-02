# Ciclo de Desenvolvimento

## Visão Geral

O Ciclo de Desenvolvimento no `FlowED` é focado na criação e implementação de novas funcionalidades. Ele abrange desde a inicialização de features em branches específicas até a integração dessas funcionalidades na branch `develop` e, eventualmente, em uma branch `release` para estabilização.

## Etapas do Ciclo de Desenvolvimento

1. **Criação de Feature Branch:**
   - Cada nova funcionalidade é desenvolvida em uma branch específica, criada a partir da `develop`.
   - O desenvolvedor inicia o trabalho isoladamente, garantindo que a nova funcionalidade não impacte outras partes do projeto durante o desenvolvimento.

2. **Desenvolvimento Isolado:**
   - O desenvolvedor implementa e testa a nova funcionalidade dentro da feature branch.
   - Testes unitários e outros tipos de validação devem ser realizados localmente para garantir que a funcionalidade está funcionando conforme esperado.

3. **Integração na Develop:**
   - Após a conclusão e verificação da funcionalidade, a feature branch é integrada na `develop` por meio de um pull request.
   - A integração inclui revisões de código e execução de testes automatizados para garantir a estabilidade da branch `develop`.

4. **Testes na Develop:**
   - Uma vez integrada, a funcionalidade é testada no contexto da branch `develop` para verificar a integração com outras funcionalidades existentes.
   - Bugs ou ajustes são realizados diretamente na `develop` ou em uma nova iteração da feature branch.

5. **Preparação para Release:**
   - Após a estabilização da `develop`, é considerada a criação de uma branch `release`, marcando o final do Ciclo de Desenvolvimento e o início do Ciclo de Homologação.
