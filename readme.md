## ❓Case para o desafio

O GCB Academy decidiu propor um desafio para o time de desenvolvedores, desenvolver um algorítimo que fosse capaz de juntar em grupos de estudo de 3 devs para que pudessem construir projetos juntos durante um tempo.

Existem algumas especificidades da forma que esse algorítimo deve formar os grupos, são essas:

- Cada grupo de estudo deve conter no máximo 3 pessoas;
- Em cada grupo, é necessário que existam 2 desenvolvedores Front-end e 1 Back-end;
- O grupo deve ser formado pelas pessoas que menos participaram de grupos de estudos;
- O algorítimo deve sortear quantos grupos forem pedidos;
- É necessário pegar aleatoriamente as pessoas para o grupo;
- Gerar os grupos mostrando os 3 participantes de cada e suas respectivas informações.

A sua missão é: Construir um algorítimo que seja capaz de resolver esse problema.

## ➡️ Exemplo

```js
const students = [
  { name: "Jonny", times: 3, stack: "BACK" },
  { name: "Maria", times: 0, stack: "FRONT" },
  { name: "Selena", times: 2, stack: "BACK" },
  { name: "Mathew", times: 1, stack: "FRONT" },
  { name: "Lucas", times: 1, stack: "FRONT" },
  { name: "Ana", times: 0, stack: "BACK" },
  { name: "Allan", times: 0, stack: "BACK" },
];

// call your function/method
const result = run({ array: students, groups: 5 });

// show result
console.log(result);

// [
//   [
//     { name: 'Ana', times: 3, stack: 'BACK' },
//     { name: 'Maria', times: 4, stack: 'FRONT' },
//     { name: 'Lucas', times: 4, stack: 'FRONT' }
//   ],
//   [
//     { name: 'Allan', times: 2, stack: 'BACK' },
//     { name: 'Maria', times: 4, stack: 'FRONT' },
//     { name: 'Mathew', times: 4, stack: 'FRONT' }
//   ],
//   [
//     { name: 'Allan', times: 2, stack: 'BACK' },
//     { name: 'Mathew', times: 4, stack: 'FRONT' },
//     { name: 'Maria', times: 4, stack: 'FRONT' }
//   ],
//   [
//     { name: 'Ana', times: 3, stack: 'BACK' },
//     { name: 'Lucas', times: 4, stack: 'FRONT' },
//     { name: 'Maria', times: 4, stack: 'FRONT' }
//   ],
//   [
//     { name: 'Ana', times: 3, stack: 'BACK' },
//     { name: 'Mathew', times: 4, stack: 'FRONT' },
//     { name: 'Lucas', times: 4, stack: 'FRONT' }
//   ]
// ]
```

<aside>
💡 Não leve o resultado do exemplo acima como certo, o algorítimo deve sortear aleatoriamente os participantes que menos foram para o grupo de estudos, portanto, nem toda vez o resultado será o mesmo.

</aside>
