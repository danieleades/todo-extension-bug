# Todo Extension Tutorial Bug

this repo is a reproduction of a bug.

The 'TODO' extension example fails to build a PDF if the content of a 'todo' vertex contains a glossary term.

To build, run-

        poetry run make latexpdf

you should see the following output-

```
...
Exception occurred:
  File ".../site-packages/docutils/nodes.py", line 624, in __getitem__
    return self.attributes[key]
KeyError: 'refdocname'
...
```
