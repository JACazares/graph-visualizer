# graph-visualizer

A small interactive graph visualizer built with D3.js.

## Usage

1. Open `index.html` in a modern web browser.
2. Paste your graph description into the text box and click **Draw Graph**.

The expected input format is:

```
N
x1 y1 [label1]
x2 y2 [label2]
...
x{N-1} y{N-1} [label{N-1}]
[label of node 1]
[label of node 2]
...
[label of node N]
```

- The first line contains `N`, the number of nodes (nodes are assumed to be numbered 1..N).
- The next `N-1` lines describe edges. Each line contains the source and target node numbers separated by spaces and an optional third value used as the edge label.
- Optionally, the following `N` lines specify labels for nodes 1..N. If these lines are omitted, nodes will be labeled with their number.

After parsing the input, the graph will appear in the SVG area. Nodes can be dragged around and the edges will follow.

