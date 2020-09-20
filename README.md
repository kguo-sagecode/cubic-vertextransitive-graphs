# cubic-vertextransitive-graphs
The census of small connected cubic vertex-transitive graphs in graph6 strings. 

The census of small connected cubic vertex-transitive graphs is a joint project by Primož Potočnik, Pablo Spiga, and Gabriel Verret, where they computer all cubic, vertex transitive graphs on n vertices, for n up to 1280. The citations and link to the census are at the end of this file.

The census is given in Magma code. With the permission of the authors, I have converted it to graph6 strings and made it freely avaiable here, so that it can be more easily accessed in sage. Each file cubicvta-bg6.txt consists of the graphs on n vertices, n from a to b inclusive, and are files where each line is the graph6_string of a cubic vertex transitive graphs. It can be used in sage as follows:

sage: f = open("cubicvt4-300g6.txt","r")
sage: aa = f.readlines()
sage: f.close()
sage: thegraphs = [Graph(now.strip("\n")) for now in aa]

This will create a list called "thegraphs" of Graph objects in sage. Note that each line is a graph6_string, but when read in, one must remove the newline character.



Link to the census: http://staff.matapp.unimib.it/~spiga/census.html
References:
P. Potočnik, P. Spiga, G. Verret, Cubic vertex-transitive graphs on up to 1280 vertices, Journal of Symbolic Computation 50 (2013), 465-477.
P. Potočnik, P. Spiga, G. Verret, Bounding the order of the vertex-stabiliser in 3-valent vertex-transitive and 4-valent arc-transitive graphs, arXiv:1010.2546v1 [math.CO].
