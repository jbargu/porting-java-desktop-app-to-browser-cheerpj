# Porting Java desktop app to a browser - Tabletop Framework Games

An example of a Java desktop application (Swing and multithreading) executed in the browser using [CheerpJ 3.0](https://labs.leaningtech.com/blog/cheerpj-3.0). Surely no one has ever thought about running Java in the browser, [have they](https://www.java.com/en/download/help/enable_browser.html)?  

A blog post about more details can be found on [the blog](https://jbargu.github.io/en/post/porting-java-to-wasm-tag-framework/).

## Setup

1. download [the TAG framework](https://github.com/GAIGResearch/TabletopGames)
2. apply patches in the `tag.patch` file
3. execute `mvn package` to generate a `FrontEnd.jar` in `target/` directory.
4. copy it into this folder.

## Run

```bash
npx http-server -p 8080
```

Visit 127.0.0.1:8080 to see the JAR running in the browser.
