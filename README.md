# SkillMatch JS

## Sobre o que é o projeto?

É simulador que compara habilidades com os requisitos de várias vagas de front-end júnior. Basicamente, o programa mostra:
- quanto o candidato tem de compatibilidade com cada vaga (em %);
- quais habilidades ele já tem;
- o que falta aprender;
- qual é a melhor vaga para ele;
- um plano de estudo baseado nas vagas.

## Qual o objetivo?

O objetivo do projeto é estudar e entender melhor os conceitos que aprendi no Módulo 01:
- como raciocinar em lógica de programação;
- JavaScript na prática;
- tipos de dados (strings, números, arrays, objetos);
- if/else e outros jeitos de fazer decisões;
- operadores matemáticos e lógicos;
- entender escopo (const, let, var);
- laços de repetição (forEach, for);
- funções e arrow functions;
- trabalhar com arrays e seus métodos;
- objetos e classes;
- herança em classes;
- this dentro de métodos;
- callbacks e closures;
- Promises e async/await;
- versionamento com GitHub;
- Kanban pra organizar tarefas.

## Como usar?

Não precisa do Node.js, basta fazer isso:

1. Abrir o Chrome (ou Firefox).
2. Apertar F12 ou Ctrl + Shift + J.
3. Ir pra aba Console.
4. Copiar todo o código do arquivo skillmatch.js.
5. Colar no console.
6. Apertar Enter.

Pronto! Daí você consegue rodar os comandos:

```javascript
// Ver compatibilidade com a primeira vaga
const resultado = calcularCompatibilidade(candidato.habilidades, vagas[0].requisitos);
console.log(resultado);

// Saber se 75% é alta, média ou baixa
classificarCompatibilidade(75);  // "Média Compatibilidade"

// Descobrir qual vaga é a melhor
encontrarMelhorVaga(candidato, vagas);

// Ver o que eu preciso estudar
gerarRecomendacaoEstudo(candidato, vagas);

// Mostrar mensagem customizada (callback)
finalizarAnalise(candidato.nome, exibirMensagemFinal);

// Contar quantas vezes analisei (closure)
const contador = criarContadorDeAnalises();
contador();  // 1
contador();  // 2
contador();  // 3

// Simular carregamento de vagas de um servidor (async/await)
iniciarSistema();
```

## Estrutura dos arquivos

```txt
skillmatch-js/
│
├── skillmatch.js
└── README.md
```

## O que implementei?

### Dados que usei (RF01 e RF02)
- ✅ Um objeto meu (candidato) com minhas habilidades
- ✅ 5 vagas diferentes com seus requisitos

### Funções principais (RF03 a RF07)
- ✅ calcularCompatibilidade() - compara habilidades
- ✅ classificarCompatibilidade() - diz se é alta/média/baixa
- ✅ listarHabilidadesFaltantes() - mostra o que falta
- ✅ encontrarMelhorVaga() - acha a vaga mais compatível
- ✅ gerarRecomendacaoEstudo() - lista tudo que preciso estudar

### Métodos de array (RF08)
- ✅ filter() - seleciono só o que preciso
- ✅ includes() - verifico se algo existe
- ✅ map() - transformo dados
- ✅ reduce() - comparo pra achar o maior
- ✅ forEach() - passo por cada item

### Classes e herança (RF09-RF11)
- ✅ class Vaga - criei um molde pra vaga
- ✅ class VagaFrontEnd - estendi Vaga pra vagas de front-end
- ✅ constructor - inicializa as vagas
- ✅ exibirResumo() e exibirNivel() - métodos das classes
- ✅ this - uso pra refernciar propriedades
- ✅ extends e super - pra fazer herança

### Coisas avançadas (RF12-RF14)
- ✅ finalizarAnalise() - função que recebe outra função (callback)
- ✅ criarContadorDeAnalises() - função que "lembra" do contador (closure)
- ✅ buscarVagasSimuladas() - simula uma requisição de servidor (Promise)
- ✅ iniciarSistema() - espera a resposta do servidor (async/await)

## Ferramentas que usei

**VS Code** - meu editor
- Live Server - roda servidor local
- Prettier - formata o código automaticamente
- ESLint - me avisa se tem algo errado
- GitLens - mostra o histórico dos commits

## Branches do projeto

- main - versão final pronta
- develop - onde testo as coisas
- feat/analise-vagas - as funções principais
- docs/readme - esse arquivo

## Autora do projeto

Maria Izabel de Lima - Estudando desenvolvimento front-end

