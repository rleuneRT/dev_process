## Tools

### WIKI/GITBOOK

- suggest to extensively use wiki in markdown format to write
  - stories
  - issues
  - specs
- you can use the amazing gitbook tool to convert the markdown docs to an ebook (see this one)

### plugins to gitbook

#### table of contents

- [plugin](https://plugins.gitbook.com/plugin/atoc)

#### gdocs inclusion

see [link](https://plugins.gitbook.com/plugin/googledocs)

example
```
http://spreadsheets.google.com/ccc?key={key}&hl=en
```

#### mermaid

- [plugin](https://plugins.gitbook.com/plugin/mermaid2)
- [info about mermaid](http://knsv.github.io/mermaid/)
- 

#### chart

```
{% chart %}
{
    // NOT need to specified `bindto` here
    data: {
        type: 'bar',
        columns: [
            ['data1', 30, 200, 100, 400, 150, 250],
            ['data2', 50, 20, 10, 40, 15, 25]
        ],
        axes: {
            data2: 'y2'
        }
    },
    axis: {
        y2: {
            show: true
        }
    }
}
{% endchart %}
```

{% chart %}
{
    // NOT need to specified `bindto` here
    data: {
        type: 'bar',
        columns: [
            ['data1', 30, 200, 100, 400, 150, 250],
            ['data2', 50, 20, 10, 40, 15, 25]
        ],
        axes: {
            data2: 'y2'
        }
    },
    axis: {
        y2: {
            show: true
        }
    }
}
{% endchart %}

