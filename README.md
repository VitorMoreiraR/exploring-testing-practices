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

**1. Repositório selecionado:** `(https://github.com/hectorcanto/pytest-samples)`

**2. Explicação:** `Os dados do TestMiner mostram um panorama geral da qualidade e da organização dos testes dentro de um repositório. Nesse caso, o projeto possui 8 arquivos de código fonte e 9 arquivos de teste, o que indica uma boa cobertura, já que há praticamente um arquivo de teste para cada parte relevante do sistema. Além disso, existem 6 arquivos classificados como test helpers, que são utilitários usados para evitar repetição de código nos testes, e 1 arquivo de mock, utilizado para simular dependências externas, como APIs ou bancos de dados. Também aparecem 3 testes do tipo smoke, que são testes simples e rápidos usados para verificar se o sistema está funcionando minimamente antes de executar testes mais complexos.

Na seção de “Tests”, o TestMiner categoriza os testes em diferentes tipos, como testes efetivos, testes com factories, testes aproximados, testes focados em asserts e o arquivo conftest, que é característico do pytest e serve para definir configurações e fixtures compartilhadas. Isso indica que o projeto utiliza boas práticas modernas de teste, com reutilização e organização.

Por fim, as dependências listadas, como pytest, pytest-cov, faker e requests-mock, reforçam que o projeto utiliza ferramentas avançadas para testes, incluindo geração de dados fictícios, medição de cobertura e simulação de requisições HTTP.`
