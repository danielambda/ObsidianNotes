---
tags:
  - Math
  - DiscreteMath
  - GraphTheory
slide: "14.26"
---
## Algorithm
1. $\forall u,v\in V:f(u,v)=0$
2. While there is a [[Walk|path]] $p$ from $s$ to $t$ *ignoring the direction of the edges* such that $\forall (u,v)\in p:c(u,v)>f(u,v)$
	1. find $c_f(p)=\min\{c(u,v)-f(u,v)>0|(u,v)\in p\}$
	2. put $f(u,v):=f(u,v)+c_f(p),$ if $\overline{(u,v)}\in p$
	3. put $f(u,v):=f(u,v)-c_f(p),$ if $\overline{(v,u)}\in p$
## Code 
``` 
FordFulkersonMethods(G, s, t)
	initialize flow f to 0
	while there exists an augmenting path p in the residual network G_f
		augment flow f along p
	return f
```

``` C#
void FordFulkerson(Graph g, Vertex s, Vertex t)
{
	foreach (var edge in g.Edges)
		edge.Flow = 0;
	
	while (g.ResidualNetwork.ExistsPathFromTo(s, t, out var p))
	{
		var c = g.Edges
			.Where(e => p.Contains(e))
			.Min(e => e.Capacity);
		
		foreach (var edge in p)
			edge.Flow += g.Edges.Contains(edge) 
				? c
				: -c;
	} 

	return someRandomFlowThatIsNotEvenInitialisedInCormen;
}
```