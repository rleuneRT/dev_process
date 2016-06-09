## Tools

### WIKI/GITBOOK

- suggest to extensively use wiki in markdown format to write
  - stories
  - issues
  - specs
- you can use the amazing gitbook tool to convert the markdown docs to an ebook (see this one)

### plugins to gitbook

book.json file

```json
{
    "gitbook": ">=2.0.0",
    "plugins": ["edit-link","googledocs","atoc","github","gitbookcode","chart","image-captions","mermaid2","highlight2","codeblock","zingchart"],
    "pluginsConfig": {
            "edit-link": {
                "base": "https://github.com/Incubaid/dev_process/edit/master/",
                "label": "Edit This Page"
            },
    "googledocs": {
            "rm": "minimal",
            "frameborder": "0",
            "width": "100%",
            "height": "500px",
            "noembed": "new window"
        },
     "atoc": {
            "addClass": true,
            "className": "atoc"
        },
    "chart": {
            "type": "highcharts"
        },
    "github": {
            "url": "https://github.com/Incubaid/dev_process"
        }
    }
}




```

is example file to be put in gitbook (in root of folder), enables next plugins.

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

```
{% mermaid %}
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
{% endmermaid %}
```

{% mermaid %}
graph TD;
  A-->B;
  A-->C;
  B-->D;
  C-->D;
{% endmermaid %}


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

#### include codeblock

- [plugin](https://plugins.gitbook.com/plugin/include-codeblock)

#### include

to include other markdown docs, ideal to avoid repetition

- [plugin](https://plugins.gitbook.com/plugin/include)

to use \!\INCLUDE "file.md"



#### zingchart

docs see
https://www.zingchart.com/docs/

{% zingchart width=300, height=300 %}
{
    "type":"bar",  
    "series":[  
        { "values": [35, 42, 67, 89]},
        { "values": [28, 40, 39, 36]}
    ]
}
{% endzingchart %}

