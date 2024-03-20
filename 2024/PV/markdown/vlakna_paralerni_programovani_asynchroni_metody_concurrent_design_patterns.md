<div align="center">
  <img src="https://www.spsejecna.cz/ci/SPSE-Jecna_Logotyp.png" alt="SPSE Jecna Logotyp" width="400" style="margin: 20px;">
</div>

# Maturitní Téma: Název tématu

- **Anki Flashcards**: [![Anki Flashcards](https://img.shields.io/badge/Anki-Flashcards-1f425f.svg)](https://ankiweb.net/shared/info/)
- **Autoři**: Ondřej Kulhavý, Maksym Kintor

## O čem mluvit a kody

1) traditional VS Paralaleni programovani 
2) Vlakno & process
3) memory issues, shared memory between threads  
3) Asynchronous methods 
5) Concurrent design patterns
- thread pool

## Video

Odkaz na případné video, které ilustruje nebo doplňuje téma

## Obsah

### Rozcestník

[Vlákna](#vlákna)  
[Paralelní programování](#paralelní_programování)  
[Asynchroni metody](#asynchroni_metody)  
[Concurrent design patterns](#concurrent_design_patterns)

### Samotný Obsah

## Vlákna

- Vlákno je proces vykonávání činnosti. Můžeme je spustit několik najednou a aplikace bude vykonávat několik akcí najednou.
- Každá aplikace je minimálně jedno main vlákno, ty co my vytváříme už jsou vedlejší.
- Vlákna běží na jádrech (pokud více jádrový procesor, tak se rozdělí)
- Hodně vláken neznamená větší efektivita, oni se budou rušit a práce se zpomalí.
- Vlákna se mohou přerušovat, respekt dochází k přeskočení na jiné vlákno, z toho důvodu je nutné uzamčení pro ostatní vlákna, dokud se nedokončí toto nikdo jiný k němu nemůže přistupovat

#### Příklad c#

```csharp
static void Worker(int iterations)
{
    //some task
    for (int i = 0; i < iterations; i++)
    {
        Console.WriteLine($"Child thread working: {i}");
    }
}

public static void Main(string[] args)
{

  int iterations = 10;

  //create new thread and use lambda to pass parameter to Worker method
  Thread thread = new Thread(() => Worker(iterations));
  //run worker task
  thread.Start();

  //run main thread task
  for (int i = 0; i < iterations; i++)
  {
      Console.WriteLine($"Main thread working: {i}");
  }
}
```

### Příklad Python

```python
import threading

def worker(iterations):
    for i in range(iterations):
        print(f"Child thread working: {i}")

iterations = 10

# create new thread and use lamba to pass parameter to Worker method
thread = threading.Thread(target=worker, args=(iterations,))
# run worker task
thread.start()

# run main thread task
for i in range(iterations):
    print(f"Main thread working: {i}")
```
