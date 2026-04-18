# Explorando Práticas de Teste

Neste exercício, vamos explorar práticas de teste em sistemas reais utilizando a ferramenta [TestMiner](https://andrehora.github.io/testminer).

O TestMiner permite visualizar e analisar testes de software em repositórios do GitHub, fornecendo dados sobre como os projetos organizam seus testes, como eles evoluem entre versões e quais bibliotecas de teste são utilizadas.
Explore a ferramenta antes de começar para se familiarizar com seu funcionamento.

---

## Passo 1: Selecionar um repositório

Escolha um repositório real que possua testes escritos na linguagem de sua preferência.
Abaixo estão alguns links para ajudá-lo a encontrar projetos interessantes:

- **Python:** https://github.com/topics/python?l=python
- **JavaScript:** https://github.com/topics/javascript?l=javascript
- **TypeScript:** https://github.com/topics/typescript?l=typescript
- **Java:** https://github.com/topics/java?l=java

## Passo 2: Explorar o repositório selecionado

Busque o repositório escolhido no [TestMiner](https://andrehora.github.io/testminer) e analise os dados de teste gerados pela ferramenta.

## Passo 3: Explicar uma prática de teste

Com base nos dados obtidos, selecione uma prática ou dado de teste relevante e explique-o com suas próprias palavras.

---

## Instruções de entrega

1. Faça um `fork` deste repositório (saiba mais sobre forks [aqui](https://docs.github.com/pt/pull-requests/collaborating-with-pull-requests/working-with-forks/fork-a-repo)).
2. Responda às questões abaixo diretamente neste arquivo `README.md` do seu fork. Pode adicionar imagens para enriquecer sua explicação.
3. No Moodle, submeta apenas a URL do seu fork.

---

## Respostas

**1. Repositório selecionado:** `https://github.com/PaperMC/Paper`

**2. Explicação:** `Os dados do TestMiner do repositório PaperMC/Paper mostram que é um projeto bem grande, com 4289 arquivos de código e 205 testes, ou seja, tem bastante teste, mas não na mesma proporção do código. Os testes estão organizados por partes do sistema, como item, block e plugin, o que ajuda a manter tudo mais claro e fácil de manter. Também existem 37 arquivos de apoio, que servem para reutilizar código nos testes e evitar repetição. Além disso, há poucos mocks, indicando que muitos testes rodam de forma mais próxima do funcionamento real do sistema. Ademais, existem alguns smoke tests e testes de CI para garantir rapidamente que nada quebrou. No geral, é um projeto com testes bem organizados e focados no que realmente importa, sem tentar cobrir absolutamente tudo.

O repositório PaperMC/Paper possui poucos mocks nos testes principalmente por causa da natureza do projeto ele é um servidor completo de Minecraft não uma biblioteca isolada em sistemas assim muitos testes precisam validar o comportamento real do servidor como interação entre blocos eventos de plugins e estado do mundo o que torna difícil e às vezes inútil simular tudo com mocks já que uma simulação não reproduziria corretamente a complexidade do ambiente por isso em vez de depender fortemente de objetos falsos o projeto tende a rodar testes mais próximos de um ambiente real ou parcialmente integrado usando apenas alguns mocks fake e dummy em situações específicas onde a dependência externa é simples ou bem controlada além disso como o código envolve muitas interações internas entre componentes e não apenas chamadas externas como APIs HTTP ou banco de dados o uso de mocks não traz tanto benefício quanto em aplicações tradicionais fazendo com que a equipe priorize testes mais realistas em vez de isolamento completo.
`
