# Nível 1: Implementação Simples

## Visão Geral

Este nível é ideal para desenvolvedores individuais ou projetos muito pequenos. Ele se concentra na simplicidade e na eficiência, utilizando uma única linha do tempo que abrange tanto o ambiente local quanto o remoto. O objetivo principal é garantir que o desenvolvedor possa manter uma rastreabilidade mínima sem sobrecarregar o processo com complexidades desnecessárias.

## Estrutura do Nível 1

- **Linha do Tempo Única:** 
  - Uma única linha do tempo, que combina o desenvolvimento local e o controle remoto.
  - Toda a atividade de desenvolvimento acontece localmente e é consolidada no repositório remoto.

- **Branch Principal:**
  - **Main:** Usada tanto para desenvolvimento quanto para a publicação direta do projeto.
  - O desenvolvedor trabalha na branch `main` localmente e, quando satisfeito com o progresso, realiza commits e push para o repositório remoto.

## Ciclo de Ações

1. **Inicialização do Repositório:**
   - Crie um repositório no GitHub com um `README.md` básico e a licença do projeto.
   - Clone o repositório para o ambiente local.

2. **Desenvolvimento Local:**
   - Trabalhe diretamente na branch `main` localmente.
   - Realize commits frequentemente, preservando um histórico claro das mudanças.

3. **Cherry-Pick para o Origin:**
   - Quando estiver pronto para consolidar o trabalho, selecione os commits mais relevantes e realize um cherry-pick desses commits para o repositório remoto (`origin`).
   - Isso garante que apenas o que é essencial seja publicado no `origin`, mantendo a simplicidade e a clareza no repositório remoto.

4. **Publicação e Versionamento:**
   - Após realizar o cherry-pick, faça o push dos commits selecionados para o `origin`.
   - Utilize versionamento semântico para marcar releases importantes.

5. **Feedback e Iteração:**
   - Caso o projeto envolva um cliente ou stakeholders, colete feedback após cada release importante.
   - Utilize esse feedback para realizar ajustes e melhorias na próxima iteração.

## Exemplos de Uso

- **Projeto Individual de Portfólio:**
  - Um desenvolvedor que deseja criar um site pessoal ou um pequeno aplicativo pode utilizar esse nível para manter as coisas simples e focadas no resultado final.

- **Projetos Acadêmicos:**
  - Alunos trabalhando em pequenos projetos acadêmicos podem adotar essa estrutura para gerenciar seu código sem a complexidade de múltiplas branches e processos.

## Vantagens do Nível 1

- **Simplicidade:** Ideal para quem precisa de um fluxo de trabalho direto e sem complicações.
- **Eficiência:** Focado na produção rápida e no feedback iterativo, sem distrações.
- **Documentação Básica:** Facilita a entrada em práticas de versionamento e controle de código, preparando o desenvolvedor para cenários mais complexos no futuro.

## Ferramentas Recomendadas

- **GitHub:** Para controle de versão e repositório remoto.
- **Editor de Código Simples (VSCode, Atom):** Facilita a codificação com suporte para Git integrado.

