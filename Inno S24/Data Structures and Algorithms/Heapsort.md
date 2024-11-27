---
id: Heapsort
aliases: []
tags:
  - Algorithms
  - DataStructures
---
## Algorithm
```cs
void Heapsort<T>(T[] items, Func<T, int> toInt)
{
    Heap heap = BuildMaxHeap(items, toInt);

    for (int i = (a.Length / 2) - 1; i > 2; i--)
    {
        Swap(a, 0, i);
        heap.size--;
        MaxHeapify(heap, 0);
    }
}
```
- Check MaxHeapify in [[Binary Heap]]

