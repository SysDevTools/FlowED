# Linha do Tempo das Releases Locais de Usuário

## Visão Geral

As releases locais de usuário são branches temporárias criadas a partir da `release` ou `develop` para que cada desenvolvedor possa trabalhar de forma independente, aplicando correções ou realizando testes sem interferir nas branches principais.

## Ciclo de Vida

1. **Criação e Uso:**
   - Um desenvolvedor cria uma branch local para testar ou ajustar funcionalidades específicas, sem impactar a `develop` ou a `release`.
   - Essa branch permite ao desenvolvedor experimentar e corrigir problemas localmente antes de fazer merges significativos.

2. **Integração com a Release ou Develop:**
   - Após realizar testes locais, o desenvolvedor pode integrar as mudanças na branch `release` ou `develop`.
   - A branch local é então deletada, mantendo o repositório limpo e organizado.

3. **Armazenamento Temporário:**
   - Essas branches são temporárias e devem ser deletadas após o merge para evitar desorganização no repositório.
   - Elas são usadas para manter a rastreabilidade das mudanças até que estejam prontas para ser integradas nas branches principais.

## Referências

- Consulte o [documento sobre níveis de implementação](./docs/pt-br/levels/simple.md) para entender como as releases locais podem ser usadas em diferentes contextos.
- Para mais detalhes sobre o ciclo de desenvolvimento, veja o [documento de ciclos](./docs/pt-br/cycles/development.md).
