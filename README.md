# Queue


### Declaração e inicialização da fila
```csharp
Queue<int> fila = new Queue<int>();
```
Neste trecho, uma nova fila de inteiros é criada e inicializada. Aqui está a declaração de uma fila vazia que pode armazenar valores inteiros.

### Adição de elementos na fila
```csharp
fila.Enqueue(2);
fila.Enqueue(4);
fila.Enqueue(6);
fila.Enqueue(8);
```
Estas linhas adicionam valores inteiros à fila. Por exemplo, `fila.Enqueue(2)` adiciona o valor inteiro 2 à fila, `fila.Enqueue(4)` adiciona 4, e assim por diante. Após essas operações, a fila contém os valores {2, 4, 6, 8}.

### Iteração sobre a fila usando um loop foreach
```csharp
foreach(int item in fila)
{
    Console.WriteLine(item);
}
```
Este loop itera sobre todos os elementos presentes na fila. Para cada elemento na fila, o loop imprime o valor do elemento no console. Por exemplo, se a fila contém os valores {2, 4, 6, 8}, este loop imprimirá cada um desses valores em linhas separadas no console.

### Remoção de um elemento da fila
```csharp
Console.WriteLine($"Removendo o elemento: {fila.Dequeue()}");
```
Esta linha remove o primeiro elemento da fila (o mais antigo) e o imprime no console junto com uma mensagem informativa. Por exemplo, se a fila inicialmente contém os valores {2, 4, 6, 8}, após essa operação, o valor 2 será removido da fila e impresso no console.

### Adição de um novo elemento na fila
```csharp
fila.Enqueue(10);
```
Esta linha adiciona um novo elemento (valor 10) ao final da fila. Após essa operação, a fila conterá os valores {4, 6, 8, 10}.

### Iteração sobre a fila novamente
```csharp
foreach(int item in fila)
{
    Console.WriteLine(item);
}
```
Este loop itera sobre todos os elementos presentes na fila após a remoção e a adição de novos elementos. Ele imprime cada valor de elemento restante na fila em linhas separadas no console. Se a fila contiver os valores {4, 6, 8, 10}, este loop imprimirá cada um desses valores.
