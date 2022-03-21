---
theme: shibainu
background: https://source.unsplash.com/collection/94734566/1920x1080
class: 'text-center'
highlighter: shiki
lineNumbers: false
favicon: https://images.unsplash.com/photo-1561106230-04eb4ff57511?auto=format&fit=crop&w=64&q=80
info: |
  ## Micro-frontends & BFFs
  An overview of Micro-frontends and BFF architectures
drawings:
  persist: false
layout: section
src: slides/intro.md
---

---
layout: default-7
src: slides/presentation-overview
---

---
layout: default-6
src: slides/the-old-way
---

---
layout: default-3
---

# Monolithic Front-end

`my-ocf-app`

<!-- ./components/SelfPromo.vue -->
<SelfPromo />

---

# Diagrams

You can create diagrams / graphs from textual descriptions, directly in your Markdown.

<div class="grid grid-cols-3 gap-10 pt-4 -mb-6">

```mermaid {scale: 0.5}
sequenceDiagram
    Alice->John: Hello John, how are you?
    Note over Alice,John: A typical interaction
```

```mermaid {theme: 'neutral', scale: 0.8}
graph TD
B[Text] --> C{Decision}
C -->|One| D[Result 1]
C -->|Two| E[Result 2]
```

```plantuml {scale: 0.7}
@startuml

package "Some Group" {
  HTTP - [First Component]
  [Another Component]
}

node "Other Groups" {
  FTP - [Second Component]
  [First Component] --> FTP
}

cloud {
  [Example 1]
}


database "MySql" {
  folder "This is my folder" {
    [Folder 3]
  }
  frame "Foo" {
    [Frame 4]
  }
}


[Another Component] --> [Example 1]
[Example 1] --> [Folder 3]
[Folder 3] --> [Frame 4]

@enduml
```

</div>

[Learn More](https://sli.dev/guide/syntax.html#diagrams)
