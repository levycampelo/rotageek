---
title: "Blog estático com Hugo"
weight: 1
date: 2024-07-23T08:48:36-03:00
authors:
  - levy
tags:
  - Blog Hugo
draft: true
---
HUGO é um gerador de sites estáticos escrito com Golang que vem ganhando muita visibilidade devido a sua rapidez para gerar/compilar conteúdos. Ao lado de Jekyll (escrito em Ruby) ambos os geradores disponibilizam uma gama enorme de recursos para que você possa criar um site ou um blog em minutos.

### Instalar o pacote webpack:
```
# apt install nodejs
```

### Instalar o curl:
```
# apt install curl
```

### Criar o novo website:
```
hugo new site <name of site>
cd <name of site>
cd themes
curl -L https://github.com/thegeeklab/hugo-geekblog/releases/latest/download/hugo-geekblog.tar.gz | 
tar -xz -C themes/hugo-geekblog/ --strip-components=1
```

### Ajustar o arquivo config.toml
```
baseURL = "http://localhost"
title = "Geekblog"
theme = "hugo-geekblog"

pluralizeListTitles = false

# Geekblog required configuration
pygmentsUseClasses = true
pygmentsCodeFences = true
disablePathToLower = true

# Needed for mermaid shortcodes
[markup]
  [markup.goldmark.renderer]
    unsafe = true
  [markup.tableOfContents]
    startLevel = 1
    endLevel = 9

[taxonomies]
  author = "authors"
  tag = "tags"

[mediaTypes]
  [mediaTypes."application/atom+xml"]
    suffixes = ["xml"]

[outputFormats]
  [outputFormats.Atom]
    name = "Atom"
    mediaType = "application/atom+xml"
    baseName = "feed"
    isPlainText = false
    rel = "alternate"
    isHTML = false
    noUgly = true
    permalinkable = false

[outputs]
  home = ["HTML", "ATOM"]
  page = ["HTML"]
  section = ["HTML"]
  taxonomy = ["HTML"]
  term = ["HTML", "ATOM"]
```
### Agora vamos testar: 
```hugo server -D```

### Este comando executara seu projeto no localhost utilizando a porta 1313:
```http://localhost:1313``` 
