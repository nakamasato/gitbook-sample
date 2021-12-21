---
description: Try using GitBook for
---

# GitBook Sample

## Init GitBook

Install honkit

```
npm install honkit --save-dev
```

```
npx honkit init
```
## Plugins

```json
{
    "plugins": [
        "sequence-diagrams",
        "flowchart",
        "plantuml"
    ],
    "pluginsConfig": {
        "sequence-diagrams": {
            "theme": "simple"
        },
        "mathjax": {
            "forceSVG": true
        }
    }
}
```

```
npm install gitbook-plugin-sequence-diagrams gitbook-plugin-flowchart gitbook-plugin-plantuml
```

## Error

### `unknown block tag: content`

```
### Fundamentals: Dive a little deeper

Learn the fundamentals of MyProduct to get a deeper understanding of our main features:

{% content-ref url="kubernetes-operator/what-is-kubernetes-operator.md" %}
[what-is-kubernetes-operator.md](kubernetes-operator/what-is-kubernetes-operator.md)
{% endcontent-ref %}

{% content-ref url="kubernetes-operator/kubernetes-operator-components.md" %}
[kubernetes-operator-components.md](kubernetes-operator/kubernetes-operator-components.md)
{% endcontent-ref %}

error: error while generating page "README.md":
Template render error: (/Users/masato-naka/repos/nakamasato/gitbook-sample/README.md) [Line 14, Column 4]
  unknown block tag: content
    at Object._prettifyError (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/nunjucks/src/lib.js:36:11)
    at Template.render (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/nunjucks/src/environment.js:538:21)
    at Environment.renderString (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/nunjucks/src/environment.js:380:17)
    at Promise.apply (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/q/q.js:1185:26)
    at Promise.promise.promiseDispatch (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/q/q.js:808:41)
    at /Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/q/q.js:1411:14
    at runSingle (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/q/q.js:137:13)
    at flush (/Users/masato-naka/repos/nakamasato/gitbook-sample/node_modules/q/q.js:125:13)
    at processTicksAndRejections (node:internal/process/task_queues:78:11)
```



## Getting Started

**Got 2 minutes?** Check out a video overview of our product:

### Guides: Jump right in

Follow our handy guides to get started on the basics as quickly as possible:

[basics.md](kubernetes/basics.md)

### Fundamentals: Dive a little deeper

Learn the fundamentals of MyProduct to get a deeper understanding of our main features:

[what-is-kubernetes-operator.md](kubernetes-operator/what-is-kubernetes-operator.md)


[kubernetes-operator-components.md](kubernetes-operator/kubernetes-operator-components.md)
