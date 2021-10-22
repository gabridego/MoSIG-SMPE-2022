# SMPE - Lecture 3 21/10/2021

## Comments on data visualization exercises

- Histograms are generally used for frequencies. If they are used for other purposes,
it must be clearly specified, otherwise the reader is pushed to interpret them differently.
- The explanation of what is done should be in the code. If a prediction is showed in a
graph, how it is computed should be explained in the text.
- The objective of data visualization is to infer graphically if a relation exists, then it
has to be assessed with statistical testing.
- The idea behind a graph should be clear and explained.
- One should think if a prediction or fit makes sense (for ex., negative number of errors).
- Never exaggerate with superlative, they do not make an assumption stronger. Let the graphs
talk.

## Data management

- Data need to be link together if they are related and in different tables.
- When reading data, one must check data types. CSV is a light format but lacks this
information, JSON and YAML solve this issues.
- Values must be interpreted and checked, semantics matters.
- Always aim at transforming data in the best way for the goal. [cell](http://cell-lang.net/)
is a good programming language for data loading and processing.

## R and *dplyr*

- *dplyr* is a library for data manipulation.
- `%>%` represents a pipe (check [lecture3_dplyr.pdf](./lecture3_dplyr.pdf) for usage
examples).
- In *dplyr*, keywords are standard database actions, like `filter` and `select`. Advanced
instructions, like `ungroup` are available.

## Open science

- Produced knowledge should be as open as possible, *FAIR* principle
- Software is fragile and can easily disappear. Git repos are moving and are not reliable
as archives.
- *DOIs* refer to an object without knowing where it is. Do not guarantee that it will be
retrievable forever, only add additional levels of redirection.
- [Software Heritage](https://www.softwareheritage.org/) is an archive, not a git repo.
- In scientific papers, the order of the authors depend on the area of research and on culture.
The *CRediT* system is proposed, with several contributor roles.
- *binder* is used to load data from a git and launch a docker image with pre-installed
applications.
- Git is made for code, not data. Solutions are git LFS or, better, git annex.