---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
  - Programming
  - Algorithms
  - DataStructures
  - Optimization
slide: "12.76"
---
## Purpose
- Given a weighted [[Graph]], and a vertex $v$, we would like to find a [[Walk|path]] of least total weight from $v$ to each of the other vertices in the [[Graph]]
## Algorithm
1. Mark all vertices except the initial vertex as unvisited. Usually, we use infinity for this. Set the initial vertex as current.
2. For the current vertex, consider all of its unvisited neighbors and calculate their tentative distances through the current vertex (choose the smallest one). When we are done considering all of the unvisited neighbors of the current vertex, mark the current vertex as visited
3. If there are no unvisited vertices, then the algorithm is finished. Otherwise, select the unvisited vertex that is marked with the smallest tentative distance, set it as the new “current vertex”, and go back to step 2.
## Code
```C#
void Dijkstra(Graph g, Func<Edge, double> w, vertext sourse)
{
	InitializeSingleSourse(g, sourse)

	PriorityQueue<double, Vertex> queue =
	    new FibonacciHeap<double, Vertex>(g.Vertices.Select(u => 
		    new KeyValuePair<double, Vertext>
		    (
			    u.ShortestPathWeight, u
			)
		));

	while (queue.IsEmpty() is false)
	{
		u = queue.ExtractMin();

		foreach (var v in G.Adj[u])
		{
			var previousShortestPathWeight = v.ShortestPathWeight;
			Relax(u, v, w);
			if (v.ShortestPathWeight < previousShortestPathWeight)
				Q.DecreaseKey(v, v.ShortestPathWeight);
		}
	}
}

void Relax(Vertex u, Edge e, Vertex v, Func<Edge, double> w)
{
	if (v.ShortestPathWeight > u.ShortestPathWeight + w(e))
	{
		v.ShortestPathWeight = u.ShortestPathWeight + w(e);
		v.Predecessor = u;
	}
}
```
## Time Complexity
- Depends on the implementation of a [[Priority Queue]]:
	- $O(|E|\log|V|)$ when using [[Binary Heap]]
	- $O(|E|+|V|\log|V|)$ when using [[Fibonacci Heap]]
## Example
![[Pasted image 20231115133815.png]]
![[Pasted image 20231115133827.png]]
![[Pasted image 20231115133855.png]]
![[Pasted image 20231115133906.png]]
![[Pasted image 20231115133959.png]]
![[Pasted image 20231115134015.png]]
![[Pasted image 20231115134025.png]]
![[Pasted image 20231115134033.png]]
![[Pasted image 20231115134039.png]]
