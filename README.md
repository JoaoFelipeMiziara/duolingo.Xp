# duolingo-xp

!Mantenha minha sequência no Duolingo

<img src="duo.svg" width="128px"/>

Mantenedor de sequência e fazenda de XP para o Duolingo. Nunca mais seja rebaixado!

### Como usar

1. Faça um fork deste repositório

2. Acesse o Duolingo

3. Enquanto estiver logado, abra o console do navegador (Option (⌥) + Command (⌘) + J (no macOS) ou Shift + CTRL + J (no Windows/Linux))

4. Obtenha o token JWT colando isso no console e copie o valor (sem `'`)

```js

document.cookie

.split(';')

.find(cookie => cookie.includes('jwt_token'))

.split('=')[1]

 ```
  
5. Vá para o seu repositório bifurcado

6. Vá para Configurações > Segredos e Variáveis > Ações . E clique no botão Novo segredo do repositório

7. Para o nome do segredo use DUOLINGO_JWT para o valor do segredo use o valor copiado da etapa 4.

8. Vá para o seu repositório bifurcado e vá para a guia Ações e pressione o botão Eu entendo meus fluxos de trabalho, vá em frente e habilite-os

## Fluxos de trabalho

### 🔥 Mantenedor de sequência

Este projeto usa o fluxo de trabalho agendado do GitHub Actions para manter sua sequência viva. O fluxo de trabalho pode ser visto [aqui](.github/workflows/streak-keeper.yml).

### 📚 Estudo

Este repositório também pode “estudar” lições para você. Isso lhe dará XP para que você nunca mais seja rebaixado! Este fluxo de trabalho usa workflow_dispatch para acionar a sessão de estudo. Você pode escolher o número de lições a serem feitas. O fluxo de trabalho pode ser visto aqui.

## Ressalvas

- Este projeto não ajudará com suas missões diárias ou de amigos, ele só pode ganhar XP para subir no ranking da liga;
- Este projeto não fará lições ou histórias reais, apenas práticas, por isso não afetará seu caminho de aprendizagem;
#   D u o l i n g o - x p  
 