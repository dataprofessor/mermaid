# mermaid

### What is mermaid?
`Mermaid` allows the creation of diagrams using Markdown syntax.

### Simple examples
Here's a simple example:

```markdown
```mermaid
  graph TD;
      A-->B;
      A-->C;
      B-->D;
      C-->D;
```
```



The following is the output:

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

### Workflow example

```mermaid
flowchart TD
    data[(Initial Dataset)] --Data Pre-Processing-->  data2[(Curated Dataset)]
    data2 --> split{Data Splitting}
    split --> train[Training Set]
    split --> test[Test Set]
    train --Hyperparameter Optimization--> E[Cross-Validation Model]
    train --> trained[Trained Model]
    test --> trained[Trained Model]
    trained --> predicted[Predicted Y values]
```

### Reference
- Examples shown here are taken from: [Include diagrams in your Markdown files with Mermaid
](https://github.blog/2022-02-14-include-diagrams-markdown-files-mermaid/)
- [Mermaid Live Editor](https://mermaid-js.github.io/mermaid-live-editor/)
- [Mermaid Docs](https://mermaid-js.github.io/mermaid/#/)
