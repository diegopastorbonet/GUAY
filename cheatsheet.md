
# Cheatsheet

## Básico
nx.Graph()                                  # Inicializa un grafo vacío
G.add_node(1)                               # Añadir un nodo
G.add_edge(1,2)                             # Añadir una arista
G.remove_node(1)                            # Elimina el nodo 1
G.remove_edge(1,2)                          # Elimina la arista (1,2)
G.add_nodes_from([2,3])                     # Añadir una lista de nodos
G.add_edges_from([(1,2),(1,3)])             # Añadir una lista de aristas
G.add_nodes_from(H)                         # Añade los nodos de H a G (sin aristas)
G.add_edges_from(H)                         # Añade las aristas de H a G (sin nodos)
G.clear()                                   # Eliminar todos los vértices y aristas
G.nodes()                                   # Devuelve los nodos
G.edges()                                   # Devuelve las aristas
G.number_of_nodes()                         # Número de nodos
G.number_of_edges()                         # Número de aristas
G.neighbors(2)                              # Devuelve un dict_keyiterator con los vecinos de 2

## Representar
nx.draw(G)                                  # Dibujar un grafo

## Generar
nx.complete_graph(10)                       # Genera el grafo completo de 10 nodos
nx.path_graph(10)                           # Genera el path de 10 nodos
nx.complete_multipartite_graph(1, 2, 3)     # Genera el grafo tripartito completo de tamaños 1, 2 y 3
