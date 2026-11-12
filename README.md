# Cine JS

### Lógica de Programação com JavaScript

### Construa a bilheteria de um cinema em 7 etapas, praticando tipos de dados, `if`, `else` e `else if` com `alert()`, `prompt()` e `confirm()`.

---

## Sumário

- [Como começar](#mmwhevyxw18.256)
- [Etapa 1: Nome do cliente](#mmwhevyxw18.1295)
- [Etapa 2: Idade](#mmwhevyxw18.1615)
- [Etapa 3: Estudante](#mmwhevyxw18.1886)
- [Etapa 4: Classificação do filme](#mmwhevyxw18.2152)
- [Etapa 5: Entrada liberada](#mmwhevyxw18.2413)
- [Etapa 6: Preço por idade](#mmwhevyxw18.2707)
- [Etapa 7: Meia-entrada](#mmwhevyxw18.3071)
- [Desafios extras](#mmwhevyxw18.3402)
- [Referência rápida](#mmwhevyxw18.4453)
- [Erros comuns](#mmwhevyxw18.5079)
- [Documentação MDN](#mmwhevyxw18.5739)

---

## Como começar

1. Faça um **fork** deste repositório (botão **Fork** no canto superior direito do GitHub).
2. **Clone** o seu fork para o seu computador:

   ```bash
   git clone https://github.com/SEU-USUARIO/NOME-DO-REPO.git
   ```
3. Abra a pasta no VS Code.
4. Crie os arquivos do projeto:
   - Crie o arquivo **`index.html`** com a estrutura básica de uma página HTML
   - Crie o arquivo **`script.js`**. É nele que você vai programar
   - No `index.html`, adicione a tag `<script>` carregando o `script.js` **logo antes do fechamento da tag `</body>`**
   - Para testar a ligação, escreva `alert("funcionou!")` no `script.js` e abra a página. Se a mensagem aparecer, está tudo certo (depois apague essa linha)
5. Abra o `index.html` no navegador (dois cliques no arquivo ou use a extensão **Live Server** do VS Code).
6. A cada alteração no `script.js`: **salve** (Ctrl+S) e **recarregue** a página (F5).

> Abra o **console do navegador** (F12 → aba *Console*) para ver mensagens de erro e usar `console.log()`.

---

## Etapa 1: Nome do cliente

**Tarefa:** peça o nome do cliente com `prompt()`, guarde em uma variável e mostre uma mensagem de boas-vindas com o nome digitado.

**Resultado esperado:**

- O site pede o nome do cliente
- Aparece *"Boas-vindas ao Cine JS, Maria!"* com o nome digitado
- No console, `typeof` do nome mostra `string`

---

## Etapa 2: Idade

**Tarefa:** peça a idade do cliente com `prompt()`, converta o valor com `Number()` e mostre quantos anos ele terá daqui a 1 ano.

**Resultado esperado:**

- Digitando `20`, aparece *"Daqui a 1 ano você terá 21 anos"*

---

## Etapa 3: Estudante

**Tarefa:** pergunte com `confirm()` se o cliente é estudante e guarde a resposta em uma variável.

**Resultado esperado:**

- Clicando em **OK**, o console mostra `true`
- Clicando em **Cancelar**, o console mostra `false`
- No console, `typeof` da resposta mostra `boolean`

---

## Etapa 4: Classificação do filme

**Tarefa:** o filme é para maiores de 14 anos. Use um `if` para avisar quem tem menos de 14.

**Resultado esperado:**

- Digitando `12`, aparece *"Atenção: este filme é para maiores de 14 anos."*
- Digitando `14` ou mais, nenhuma mensagem aparece

---

## Etapa 5: Entrada liberada

**Tarefa:** complete o `if` da etapa anterior com um `else` para quem tem 14 anos ou mais.

**Resultado esperado:**

- Digitando `12`, continua aparecendo o aviso da classificação
- Digitando `14` ou mais, aparece *"Entrada liberada. Bom filme!"*
- Nunca aparecem as duas mensagens juntas

---

## Etapa 6: Preço por idade

**Tarefa:** use `if`, `else if` e `else` para definir o preço do ingresso: até 12 anos paga R$ 20, de 13 a 59 anos paga R$ 30 e a partir de 60 anos paga R$ 16.

**Resultado esperado:**

- Digitando `10` ou `12`, aparece *"Ingresso infantil: R$ 20"*
- Digitando `13` ou `59`, aparece *"Ingresso inteiro: R$ 30"*
- Digitando `60` ou mais, aparece *"Ingresso idoso: R$ 16"*

---

## Etapa 7: Meia-entrada

**Tarefa:** use a resposta da Etapa 3 em um `if`: se o cliente for estudante, o preço cai pela metade. No final, mostre o valor a pagar.

**Resultado esperado:**

- 20 anos e estudante: aparece *"Valor final: R$ 15"*
- 20 anos e não estudante: aparece *"Valor final: R$ 30"*
- 65 anos e estudante: aparece *"Valor final: R$ 8"*

---

## Desafios extras

### Desafio A: Idade inválida

**Tarefa:** antes de calcular o preço, verifique se a idade é válida. Letra, campo vazio, número negativo ou maior que 120 é inválido.

**Resultado esperado:**

- Digitando `abc`, `-5` ou `200`, aparece *"Idade inválida!"* e o preço não é mostrado
- Idades válidas continuam funcionando

### Desafio B: Pipoca

**Tarefa:** pergunte com `confirm()` se o cliente quer pipoca por R$ 12 e some ao valor final.

**Resultado esperado:**

- Com pipoca, 20 anos e não estudante: aparece *"Valor final: R$ 42"*
- Sem pipoca, o valor não muda

### Desafio C: Terça da promoção

**Tarefa:** pergunte com `prompt()` o dia da semana. Na terça, todo ingresso custa R$ 12, para qualquer idade.

**Resultado esperado:**

- Digitando `terca`, aparece *"Promoção de terça! Ingresso: R$ 12"*
- Em qualquer outro dia, o preço segue as regras normais

### Desafio D: Resumo do pedido

**Tarefa:** no final, mostre um único `alert()` com o resumo do pedido. Troque o `true` ou `false` de estudante por "sim" ou "não".

**Resultado esperado:**

- Aparece *"Cliente: Maria | Idade: 20 | Estudante: sim | Valor: R$ 15"*

---

## Referência rápida

| Função | O que faz | Devolve |
| --- | --- | --- |
| [`alert("texto")`](https://developer.mozilla.org/pt-BR/docs/Web/API/Window/alert) | Mostra uma mensagem | nada (`undefined`) |
| [`prompt("pergunta")`](https://developer.mozilla.org/pt-BR/docs/Web/API/Window/prompt) | Pede que o usuário digite algo | `string`, ou `null` se cancelar |
| [`confirm("pergunta")`](https://developer.mozilla.org/pt-BR/docs/Web/API/Window/confirm) | Pergunta sim ou não | `true` (OK) ou `false` (Cancelar) |
| [`Number(valor)`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/Number) | Converte para número | `number` ou `NaN` |
| [`isNaN(valor)`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Global_Objects/isNaN) | Verifica se **não** é um número | `true` ou `false` |
| [`typeof valor`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/typeof) | Mostra o tipo do valor | `"string"`, `"number"`, `"boolean"`... |
| [`console.log(valor)`](https://developer.mozilla.org/pt-BR/docs/Web/API/console/log_static) | Mostra o valor no console (F12) | nada |

### Operadores

| Tipo | Operadores |
| --- | --- |
| Aritméticos | `+` `-` `*` `/` |
| Comparação | `===` `!==` `>` `<` `>=` `<=` |
| Lógicos | `&&` (E) `\|\|` (OU) `!` (NÃO) |

---

## Erros comuns

| Problema | Provável causa |
| --- | --- |
| A soma junta os números (`20 + 1` vira `201`) | Esqueceu de converter o valor do `prompt()` com `Number()` |
| Aparece *"Daqui a 1 ano você terá 201 anos"* mesmo usando `Number()` | Faltaram parênteses na conta dentro do texto: use `"Daqui a 1 ano você terá " + (idade + 1) + " anos"` |
| `Uncaught SyntaxError: Unexpected token 'else'` | Tem um `else` sem `if` antes, ou falta fechar uma chave `}` |
| Quem tem 65 anos paga como adulto | A ordem do `else if` está errada, ou a condição de 60 anos nunca é testada |
| Aparecem duas mensagens quando deveria aparecer uma | Usou dois `if` separados em vez de `if` / `else` |
| O `if` sempre entra, mesmo quando não devia | Usou `=` (atribuição) em vez de `===` (comparação) |
| Nada acontece ao abrir a página | Erro de digitação no código. Abra o console (F12) e leia a mensagem em vermelho |

---

## Documentação MDN

- [Variáveis e tipos de dados](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Grammar_and_types)
- [`let`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/let) e [`const`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/const)
- [Template strings](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Template_literals)
- [`typeof`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Operators/typeof)
- [`if...else`](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Reference/Statements/if...else)
- [Expressões e operadores](https://developer.mozilla.org/pt-BR/docs/Web/JavaScript/Guide/Expressions_and_operators)
- [O que deu errado? Resolvendo problemas no JavaScript](https://developer.mozilla.org/pt-BR/docs/Learn_web_development/Core/Scripting/What_went_wrong)
