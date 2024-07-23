---
tags:
  - Math
  - DataStructures
  - Algorithms
  - GraphTheory
  - Optimization
---
## Insight
- Shortest path cannot have more than $|V|$ vertices, so it cannot have more than $|V|–1$ edges
## Code
```C#
bool BellmanFord(Graph g, Func<Edge, double> w, Vertex source)
{
	InitializeSingleSourse(g, source);

	for (int i = 1; i < g.Vertices.Count; i++)
		foreach (var (u, e, v) in g.Edges)
			Relax(u, e, v, w);

	foreach (var (u, e, v) in g.Edges)
		if (v.ShortestPathWeight > u.ShortestPathWeight + w(e))
			return false;

	return true;
}
```
## Time Complexity
- $O(|V||E|)$