---
tags:
  - DataStructures
---
## Definition
- A binary max-heap is a [[Complete Binary Tree]] that maintains the max-heap property
## Max-Heap Property
- for any parent and child nodes:
```
parent.key >= child.key
```
## Heapify Function
``` c#
void MaxHeapify(Heap heap, int currentIndex) 
{
	int l = Left(currentIndex);
	int r = Right(currentIndex);

	int maxIndex = currentIndex;

	if (l <= heap.Size && heap[l] > heap[currentIndex])
		maxIndex = l;

	if (r <= heap.Size && heap[r] > heap[largest])
		maxIndex = r;

	if (maxIndex != currentIndex)
	{
		Swap(heap, currentIndex, maxIndex);
		MaxHeapify(heap, largest);
	}
}
```
## Heap Maximum Function
``` C#
int HeapMaximum(Heap heap) => heap[0];
```
## Heap Extract Max Function
``` C#
int HeapExtractMax(Heap heap) 
{
	if (heap.size < 1) 
		throw new HeapUnderflowException();

	int max = HeapMaximum(heap);
	heap[0] = heap[heap.size - 1];
	heap.size--;
	MaxHeapify(heap, 0);

	return max;
}
```
## Heap Increase Key Function
``` C#
void HeapIncreaseKey(Heap heap, int i, int newPriority) 
{
	if (newPriority < heap[i])
		throw new ArgumentExcaption();

	heap[i] = newPriority;

	while (i > 0 && heap[Parent(i)] < heap[i]) 
	{
		Swap(heap, i, Parent(i));
		i = Parent(i);
	}
}
```
## Heap Insert Function
``` C#
void HeapInsert(Heap heap, int priority) 
{
	heap.size++;
	heap[heap.size - 1] = int.MinValue;

	HeapIncreaseKey(heap, heap.size - 1, priority);
}
```