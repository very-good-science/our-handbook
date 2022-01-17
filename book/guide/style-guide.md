# Style guide

We ask that you follow these guidelines to help us maintain a consistent style in the `Our Handbook` project.

## Leaving notes for handbook authors

If you want to leave instructions for handbook authors (the users of our template), then we try to use a special kind of [Admonition block](https://jupyterbook.org/content/content-blocks.html#notes-warnings-and-other-admonitions).
This allows us to highlight areas of the handbook that authors need to make changes to, and gives them an easy way to search for these.

As a bonus, the instruction blocks are also visible to group members browsing the work-in-progress handbook (who might not be able to understand the raw markdown code).

We use the following MyST syntax:

````md
```{admonition} FIXME Instructions
Provide guidance and instructions here

- You can use lists
- and other formatting inside
```
````

Which produces the following:

```{admonition} FIXME Instructions
Provide guidance and instructions here

- You can use lists
- and other formatting inside
```
