## ❓Case para o desafio

O GCB Academy decidiu propor um desafio para o time de desenvolvedores, desenvolver um algoritmo que fosse capaz de juntar em grupos de estudo de 3 devs para que pudessem construir projetos juntos durante um tempo.

Existem algumas especificidades da forma que esse algoritmo deve formar os grupos, são essas:

- Cada grupo de estudo deve conter no máximo 3 pessoas;
- Em cada grupo, é necessário que existam 2 desenvolvedores Front-end e 1 Back-end;
- O grupo deve ser formado pelas pessoas que menos participaram de grupos de estudos;
- O algoritmo deve sortear quantos grupos forem pedidos;
- É necessário pegar aleatoriamente as pessoas para o grupo;
- Gerar os grupos mostrando os 3 participantes de cada e suas respectivas informações.

A sua missão é: Construir um algoritmo que seja capaz de resolver esse problema.

## ➡️ Exemplo

```java
import java.util.*;

public class Main {

    // DICA: Utilize -> Random r = new Random(); int num = r.nextInt(tamanho array);
  
    public static void main(String[] args) {
      List<Student> students = new ArrayList<>();
      students.add(new Student("Jonny", 3, "BACK"));
      students.add(new Student("Maria", 0, "FRONT"));
      students.add(new Student("Selena", 2, "BACK"));
      students.add(new Student("Mathew", 1, "FRONT"));
      students.add(new Student("Lucas", 1, "FRONT"));
      students.add(new Student("Ana", 0, "BACK"));
      students.add(new Student("Allan", 0, "BACK"));
      
      // Call your function or method
      String result = run(students, 5);
      
      System.out.println("Grupos: " + result);
    }
    
  
    static class Student {
      private String name;
      private int times;
      private String stack;
      
      public Student(String name, int times, String stack) {
        this.name = name;
        this.times = times;
        this.stack = stack;
      }
      
      public String getName() {
        return name; 
      }
    
      public int getTimes() {
        return times; 
      }
      
      public String getStack() {
        return stack;
      }
  }
}

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
