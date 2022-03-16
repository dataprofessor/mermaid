# mermaid

### What is mermaid?
`Mermaid` allows the creation of diagrams using Markdown syntax.

### Simple examples
Here's a simple example:
```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```

The diagram can be much more elaborate as well:

```mermaid
flowchart TD
  A[Deploy to production] --> B{Is it Friday?};
  B --Yes--> C[Do not deploy!];
  B --No --> D[Run deploy.sh to deploy!];
  C ----> E[Enjoy your weekend!];
  D ----> E[Enjoy your weekend!];
```

# Workflow example

```mermaid
flowchart TD
  A[Inital Dataset] --> B[Pre-Processed Dataset];
  B ----> C[Data Splitting];
  C ----> D[Training set];
  C -- --> E[Test set];
  D ----> F[Cross-Validation Model];
  D ----> G[Trained Model];
  E ----> G[Trained Model];
  G ----> H[Predicted Y values];
```

### Reference
Examples shown here are taken from:
- [Include diagrams in your Markdown files with Mermaid
](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)
