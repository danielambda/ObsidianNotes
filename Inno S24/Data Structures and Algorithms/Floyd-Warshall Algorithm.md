---
tags:
  - Math
  - GraphTheory
  - DataStructures
  - Algorithms
  - Optimization
---
## Usage
- Finds shortest paths for all pairs of vertices
## Idea
- Consider candidates for intermediate vertex
![[Pasted image 20240416123938.png]]
## Code
```C#
Matrix FloydWarshall(Matrix adjacencyMatrix)
{
	int n = adjacencyMatrix.Size.Rows;
	var d = new Matrix[n + 1];
	d[0] = W;

	for (int k = 1; k <= n; k++)
	{
		d[k] = new Matrix(n, n);
		for (int i = 1; i <= n; i++)
			for (int j = 1; j <= n; j++)
				d[k][i, j] = min
				(
					d[k - 1][i, j],
					d[k - 1][i, k] + d[k - 1][k, j]
				 );
	}

	return d[n];
}
//or
Matrix SpaceEfficientFloydWarshall(Matrix adjacencyMatrix)
{
	int n = adjacencyMatrix.Size.Rows;
	
	for (int k = 0; k < n; k++)
		for (int i = 0; i < n; i++)
			for (int j = 0; j < n; j++)
				adjacencyMatrix[i, j] = Min
				(
					adjacencyMatrix[i, j],
					adjacencyMatrix[i, k] + adjacencyMatrix[k, j]
				 );
	
	return adjacencyMatrix;
}
```
## Time Complexity
- $O(|V|^3)$