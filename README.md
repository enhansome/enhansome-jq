# Awesome jq with stars

A curated list of awesome things built with the JSON processor and
*turing-complete functional language* **jq**.

* [Awesome jq  ](#awesome-jq--)
  * [Implementations](#implementations)
  * [Tools](#tools)
    * [Command-line](#command-line)
    * [Web](#web)
    * [Desktop](#desktop)
    * [Extensions](#extensions)
  * [Documentation](#documentation)
    * [Core documentation](#core-documentation)
    * [Good small specific tutorials](#good-small-specific-tutorials)
    * [Code examples](#code-examples)
    * [Documentation browsers](#documentation-browsers)
  * [Use Cases](#use-cases)
  * [Libraries and tools for jq itself](#libraries-and-tools-for-jq-itself)
  * [External libraries](#external-libraries)
  * [Podcasts and presentations](#podcasts-and-presentations)
  * [Contribute](#contribute)
  * [License](#license)

***

## Implementations

*Standalone implementations of the jq language.*

* [jq](https://jqlang.github.io/jq/) ([github](https://github.com/jqlang/jq) ⭐ 35,468 | 🐛 472 | 🌐 C | 📅 2026-08-12) – The original jq command-line JSON processor.
* [gojq](https://github.com/itchyny/gojq) ⭐ 3,795 | 🐛 18 | 🌐 Go | 📅 2026-07-20 – A jq implementation in Go.
* [jqjq](https://github.com/wader/jqjq) ⭐ 771 | 🐛 6 | 🌐 jq | 📅 2026-08-02 – jq implementation of jq
* [query-json (`q`)](https://github.com/davesnx/query-json) ⭐ 636 | 🐛 1 | 🌐 OCaml | 📅 2026-07-29 – query-json is a faster, simpler and more portable implementation of the jq language in Reason.
* [xq](https://github.com/MiSawa/xq) ⭐ 400 | 🐛 14 | 🌐 Rust | 📅 2026-07-10 – Pure rust implementation of jq
* [jq.js](https://github.com/mwh/jqjs) ⭐ 105 | 🐛 4 | 🌐 JavaScript | 📅 2026-03-17 – Pure Javascript implementation of jq
* [jaq](https://lib.rs/crates/jaq) – A jq implementation in Rust that misses some small features but is often more correct than the original.

## Tools

*jq-based JSON visualizers and explorers*.

### Command-line

* `echo '' | fzf --print-query --preview "cat *.json | jq {q}"` – An [fzf](https://github.com/junegunn/fzf) ⭐ 82,605 | 🐛 330 | 🌐 Go | 📅 2026-08-21 hack that turns it into an interactive jq explorer.
* [fq](https://github.com/wader/fq) ⭐ 10,571 | 🐛 58 | 🌐 Go | 📅 2026-08-20 – jq for binary formats
* [jnv](https://github.com/ynqa/jnv) ⭐ 6,093 | 🐛 30 | 🌐 Rust | 📅 2026-08-20 – interactive JSON filter using jq with navigation and autocompletion.
* [yq](https://github.com/kislyuk/yq) ⭐ 2,969 | 🐛 23 | 🌐 Python | 📅 2026-07-11 (and `xq`) – jq wrapper for YAML and XML documents.
* [jqp](https://github.com/noahgorstein/jqp) ⭐ 2,829 | 🐛 24 | 🌐 Go | 📅 2026-02-06 – a TUI playground for exploring jq.
* [jiq](https://github.com/fiatjaf/jiq) ⚠️ Archived – A visual command-line interactive JSON explorer with jq filters.
* [play](https://github.com/paololazzari/play) ⭐ 583 | 🐛 3 | 🌐 Go | 📅 2025-03-28 – A TUI playground to experiment with your favorite programs, such as grep, sed, awk, jq and yq.
* [faq](https://github.com/jzelinskie/faq) ⭐ 464 | 🐛 20 | 🌐 Go | 📅 2024-10-02 – CLI program that processes BSON, Bencode, JSON, TOML, XML, YAML using **libjq**.
* [jqfmt](https://github.com/noperator/jqfmt) ⭐ 409 | 🐛 8 | 🌐 Go | 📅 2026-02-03 – A code beautifier for jq.
* [jq-zsh-plugin](https://github.com/reegnz/jq-zsh-plugin) ⭐ 362 | 🐛 2 | 🌐 Shell | 📅 2025-07-23 – zsh line editor for constructing jq queries interactively.
* [jqq](https://github.com/jcsalterego/jqq/) ⭐ 319 | 🐛 0 | 🌐 Ruby | 📅 2020-05-29 – A visual command-line interactive jq explorer written in Ruby.
* [ijq](https://github.com/fiatjaf/ijq) ⭐ 30 | 🐛 0 | 🌐 Go | 📅 2022-09-21 – jq REPL with automatic variable assignment and global statements support.
* [jqsh](https://github.com/bmatsuo/jqsh) ⭐ 24 | 🐛 11 | 🌐 Go | 📅 2014-07-16 – An interactive wrapper written in Go.
* [yiq](https://github.com/zoetrope/yiq) ⭐ 16 | 🐛 0 | 🌐 Go | 📅 2021-04-22 – Like `jiq`, but using `yq` instead, so it supports YAML documents.
* [jqunit](https://github.com/mrwilson/jqunit) ⭐ 5 | 🐛 0 | 🌐 Rust | 📅 2024-03-04 – A test framework for JQ, written in Rust, on top of libjq.
* [jq-fish-plugin](https://github.com/jihchi/jq-fish-plugin) ⚠️ Archived – Inspired by [jq-zsh-plugin](https://github.com/reegnz/jq-zsh-plugin) ⭐ 362 | 🐛 2 | 🌐 Shell | 📅 2025-07-23, interactively build jq expressions in fish shell.
* [ijq](https://codeberg.org/gpanders/ijq) – Interactive jq tool. Like [jqplay](https://jqplay.org/) for the commandline.

### Web

* [jq play](https://jqplay.org/) ([github](https://github.com/jingweno/jqplay) ⭐ 845 | 🐛 27 | 🌐 TypeScript | 📅 2026-08-12) – A playground for jq with sharing capabilities.
* [jqterm](https://jqterm.com) ([github](https://github.com/remy/jqterm) ⭐ 43 | 🐛 2 | 🌐 JavaScript | 📅 2025-12-30) – Online playground - "jq as a service"
* [jqaas](https://github.com/captn3m0/jqaas) ⭐ 37 | 🐛 2 | 🌐 PHP | 📅 2024-05-27 – jq as a service, an open HTTP endpoint that executes jq queries.
* jq-finder ([github](https://github.com/fiatjaf/jq-finder) ⭐ 14 | 🐛 1 | 🌐 Elm | 📅 2018-04-27) – A multipanel, Finder-like, JSON explorer with jq filters instead of paths, uses `jq-web`.
* [jqp](https://github.com/sighrobot/jqp) ⭐ 14 | 🐛 0 | 🌐 JavaScript | 📅 2023-07-19 – A free serverless proxy for filtering JSON and CSV data using jq.
* jiq-web ([github](https://github.com/fiatjaf/jiq-web) ⭐ 9 | 🐛 1 | 🌐 HTML | 📅 2018-04-27) – `jiq`, but in a web page, uses `jq-web`.
* [query-json playground](https://query-json.netlify.app) – Web playground that uses `query-json` compiled to JavaScript.
* [jq kung fu](https://www.jqkungfu.com/) – A jq playground in WebAssembly powered by the original jq compiled with *emscripten*.

### Desktop

* [jqview](https://github.com/fiatjaf/jqview) ⭐ 369 | 🐛 1 | 🌐 Go | 📅 2020-06-30 – A jq JSON explorer with a minimalist native GUI.
* [jqi](https://nire0510.github.io/jqi/) ([github](https://github.com/nire0510/jqi) ⭐ 46 | 🐛 5 | 🌐 HTML | 📅 2018-05-01) – The almighty jq processor wrapped in a graphical UI, for Mac OSX.

### Extensions

* [bat syntax highlighting](https://github.com/jqlang/jq/wiki/bat-language-syntax) ⭐ 35,468 | 🐛 472 | 🌐 C | 📅 2026-08-12 – Syntax file to use bat to syntax highlight jq files
* [jq-mode](https://github.com/ljos/jq-mode) ⭐ 133 | 🐛 9 | 🌐 Emacs Lisp | 📅 2026-08-21 – A jq mode for Emacs.
* [jq-lsp](https://github.com/wader/jq-lsp) ⭐ 132 | 🐛 7 | 🌐 jq | 📅 2026-08-03 – jq language server. Works with VSCode, neovim and Emacs. Has syntax and scope checking, goto defintion, completion and hover documentation.
* [vim-jqplay](https://github.com/bfrg/vim-jqplay) ⭐ 124 | 🐛 2 | 🌐 Vim Script | 📅 2024-03-05 – Interactive jq playground inside Vim.
* [bro/q](https://github.com/zalando-incubator/bro-q) ⚠️ Archived – A Chrome Extension for JSON formatting and jq filtering.
* [virtual-json-viewer](https://github.com/paolosimone/virtual-json-viewer) ⭐ 83 | 🐛 3 | 🌐 TypeScript | 📅 2026-07-12 – A JSON Chrome/Firefox Extension with virtual DOM, full-text search and jq filtering.
* [vscode-jq-playground](https://github.com/davidnussio/vscode-jq-playground) ⭐ 54 | 🐛 11 | 🌐 TypeScript | 📅 2026-08-21 – A jq playground notebook extension for VS Code.
* [jq-playground.nvim](https://github.com/yochem/jq-playground.nvim) ⭐ 46 | 🐛 3 | 🌐 Lua | 📅 2026-02-13 – Interactive jq playground inside Nvim, written in Lua.
* [vscode-jq](https://github.com/wader/vscode-jq) ⭐ 32 | 🐛 2 | 🌐 TypeScript | 📅 2026-08-13 – VSCode jq extension that uses [jq-lsp](https://github.com/wader/jq-lsp) ⭐ 132 | 🐛 7 | 🌐 jq | 📅 2026-08-03. Has syntax highlight, snippets and everything jq-lsp provides.
* [vscode-jq](https://github.com/andricDu/vscode-jq) ⭐ 24 | 🐛 10 | 🌐 TypeScript | 📅 2023-01-11 – A jq extension for VS Code.
* [atom-jq](https://github.com/sanack/atom-jq) ⭐ 23 | 🐛 0 | 🌐 JavaScript | 📅 2023-01-24 – Interactive jq playground inside the Atom editor.
* `:%!jq '.'` is a Vim command that formats JSON in-place with jq (beware of any other tricks you might be thinking of).
* [jqExpress](https://plugins.jetbrains.com/plugin/23360-jqexpress) – A jq extension for JetBrains IDEs

## Documentation

*Readings about jq*.

### Core documentation

* [FAQ](https://github.com/jqlang/jq/wiki/FAQ) ⭐ 35,468 | 🐛 472 | 🌐 C | 📅 2026-08-12 – jq FAQ.
* [Cookbook](https://github.com/jqlang/jq/wiki/Cookbook) ⭐ 35,468 | 🐛 472 | 🌐 C | 📅 2026-08-12 – jq cookbook.
* [Advanced Topics](https://github.com/jqlang/jq/wiki/Advanced-Topics) ⭐ 35,468 | 🐛 472 | 🌐 C | 📅 2026-08-12 – jq advanced topics.
* [Manual](https://jqlang.github.io/jq/manual/) – jq manual (development version).

### Good small specific tutorials

* [Bash that JSON (with jq)](http://blog.librato.com/posts/jq-json).
* [JSON on the command line with jq](https://shapeshed.com/jq-json/).
* [Reshaping JSON with jq](https://programminghistorian.org/en/lessons/json-and-jq).
* [jq is sed for JSON](https://robots.thoughtbot.com/jq-is-sed-for-json).
* [Mastering jq: part 1](https://codefaster.substack.com/p/mastering-jq-part-1-59c)
* [An Introduction to JQ](https://earthly.dev/blog/jq-select/)
* [Articles exploring and using jq for data tasks](https://qmacro.org/tags/jq/)

### Code examples

* [jq at Rosetta Code](http://rosettacode.org/wiki/Category:Jq) – Dozens of algorithms written in jq .
* [Builtins](https://github.com/jqlang/jq/blob/master/src/builtin.jq) ⭐ 35,468 | 🐛 472 | 🌐 C | 📅 2026-08-12 – jq builtins coded in *jq* itself, not C.
* [Collection of jq recipes](https://remysharp.com/drafts/jq-recipes)
* [Collection of interactive jq examples](https://ishan.page/blog/2023-11-06-jq-by-example/) – Dozens of interactive jq examples (and explanations) in the browser.
* [Collection of jq oneliners](https://nntrn.github.io/jq-recipes/)

### Documentation browsers

* [jq dash docset](https://github.com/wader/jq-dash-docset) ⭐ 4 | 🐛 0 | 🌐 HTML | 📅 2025-06-02

## Use Cases

*Apps using jq in the wild*.

* [jc](https://github.com/kellyjonbrazil/jc) ⭐ 8,666 | 🐛 60 | 🌐 Python | 📅 2026-06-18 – CLI tool that converts the output of popular command-line programs and filetypes to JSON so they can be piped to jq.
* [pgJQ](https://github.com/Florents-Tselai/pgJQ) ⭐ 205 | 🐛 4 | 🌐 C | 📅 2024-12-09 – jq Postgres extension.
* [liteJQ](https://github.com/Florents-Tselai/liteJQ) ⭐ 106 | 🐛 4 | 🌐 C | 📅 2024-07-08 – jq SQLite extension.
* [jqmd](https://github.com/bashup/jqmd) ⭐ 51 | 🐛 0 | 🌐 Shell | 📅 2021-06-27 – A "literate devops" tool that allows embedding jq code, shell scripts, YAML, and JSON in a markdown document and making it executable. (A bit like R markdown or IPython notebooks, except with shell/jq/YAML/JSON, and as a CLI scripting tool rather than a GUI.)
* [jqt](https://fadado.github.io/jqt/index.html) ([github](https://github.com/fadado/jqt) ⭐ 44 | 🐛 1 | 🌐 Shell | 📅 2020-07-31) – A web template engine that uses jq as expression language.
* [bf.jq](https://github.com/MakeNowJust/bf.jq) ⭐ 43 | 🐛 0 | 🌐 JSONiq | 📅 2014-12-27 – A Brainfuck interpreter written in jq.
* [datasette-jq](https://github.com/simonw/datasette-jq) ⭐ 17 | 🐛 2 | 🌐 Python | 📅 2020-04-09 – A plugin that enables jq queries on JSON columns on [datasette](https://datasette.readthedocs.io/) deployments.
* [jtool](https://github.com/fadado/jtool) ⭐ 13 | 🐛 0 | 🌐 Shell | 📅 2019-05-12 – jq-based JSON tools for a modern shell.
* [jq-voronoi](https://github.com/hosuaby/jq-voronoi) ⭐ 11 | 🐛 0 | 🌐 jq | 📅 2021-06-18 – Implementation of Fortune’s algorithm to calculate Voronoi diagram on jq.
* [sc](https://github.com/annacrombie/sc) ⚠️ Archived – A lightweight [SoundCloud](https://soundcloud.com/) client, with a composable api, powered by jq.
* [just-dashboard](https://kantord.github.io/just-dashboard/) – A serverless app for implementing JSON-powered dashboards with JSON or YAML files (and jq filters as strings) serving as the only source of configuration.

## Libraries and tools for jq itself

*Incrementing jq capabilities*.

* [JBOL](https://github.com/fadado/JBOL) ⭐ 81 | 🐛 3 | 🌐 JSONiq | 📅 2020-07-11 – A collection of utility modules for jq (math, prelude, set, string etc.).
* [jqnpm](https://github.com/jqnpm/jqnpm) ⚠️ Archived – A jq package manager that installs modules from GitHub and runs jq scripts.
* [jq-jsonpointer](https://github.com/nichtich/jq-jsonpointer) ⭐ 19 | 🐛 3 | 🌐 JSONiq | 📅 2020-04-07 – jq module implementing JSON Pointer (RFC 6901)
* [json5.jq](https://github.com/wader/json5.jq) ⭐ 13 | 🐛 1 | 🌐 jq | 📅 2025-06-16 JSON5 implementation for jq
* [tree-sitter-jq](https://github.com/nverno/tree-sitter-jq) ⭐ 8 | 🐛 0 | 🌐 JavaScript | 📅 2025-02-26 – Tree sitter grammar implementation for Jq language
* [bigint](https://github.com/joelpurra/jq-bigint) ⚠️ Archived, [array](https://github.com/joelpurra/jq-disarray) ⚠️ Archived, [string](https://github.com/joelpurra/jq-stress) ⚠️ Archived and [other libraries](https://github.com/joelpurra?utf8=%E2%9C%93\&tab=repositories\&q=jq) – jq libraries from the author of jqnpm.
* [tar.jq](https://github.com/wader/tar.jq) ⭐ 2 | 🐛 0 | 🌐 jq | 📅 2025-09-11 tar archive creator for jq

***

## External libraries

*Using jq from other languages*.

* [gojq](https://github.com/itchyny/gojq) ⭐ 3,795 | 🐛 18 | 🌐 Go | 📅 2026-07-20 – A full jq implementation in Go, usable as a library.
* [jq.py](https://github.com/mwilliamson/jq.py) ⭐ 452 | 🐛 26 | 🌐 Python | 📅 2026-07-10 – Another jq wrapper for Python.
* [jq-web](https://github.com/fiatjaf/jq-web) ⭐ 363 | 🐛 13 | 🌐 JavaScript | 📅 2025-03-19 – jq itself compiled to JavaScript with *emscripten*. There's also an alternative at [jqdash](https://www.npmjs.com/package/jqdash).
* [node-jq](https://github.com/sanack/node-jq) ⭐ 305 | 🐛 28 | 🌐 TypeScript | 📅 2026-07-27 – A jq wrapper for Node.js.
* [pyjq](https://github.com/doloopwhile/pyjq) ⭐ 202 | 🐛 19 | 🌐 Python | 📅 2024-07-20 – A jq wrapper for Python.
* [jqr](https://github.com/ropensci/jqr) ⭐ 144 | 🐛 16 | 🌐 R | 📅 2024-12-14 – R interface to jq.
* [java-jq](https://github.com/arakelian/java-jq) ⭐ 92 | 🐛 8 | 🌐 Java | 📅 2024-04-30 – A jq wrapper for Java ([jackson-jq](https://github.com/eiiches/jackson-jq) ⭐ 310 | 🐛 42 | 🌐 Java | 📅 2026-08-21 is a Jackson extension).
* [php-ext-jq](https://github.com/kjdev/php-ext-jq) ⭐ 47 | 🐛 2 | 🌐 PHP | 📅 2022-05-26 – PHP extension for jq.
* [Ansible jq](https://github.com/moreati/jq-filter) ⭐ 24 | 🐛 4 | 🌐 Python | 📅 2024-08-16 – A jq filter for [Ansible](https://ansible.com) configuration manager.
* [jq-go](https://github.com/threatgrid/jq-go) ⭐ 22 | 🐛 4 | 🌐 Go | 📅 2017-05-31 – Golang cgo bindings for **libjq** ([jqpipe-go](https://github.com/threatgrid/jqpipe-go) ⭐ 12 | 🐛 5 | 🌐 Go | 📅 2019-11-01 is a CLI wrapper from the same people).
* [libjq-go](https://github.com/flant/libjq-go) ⭐ 16 | 🐛 5 | 🌐 Go | 📅 2020-11-26 – Golang cgo bindings for **libjq**. This one works with recent versions of jq: 1.5, 1.6+.
* [json-jq](https://github.com/dxma/perl5-json-jq) ⭐ 5 | 🐛 6 | 🌐 Perl | 📅 2022-10-28 – A jq wrapper for Perl.
* [jq-ruby](https://github.com/persona-id/jq-ruby) ⭐ 2 | 🐛 1 | 🌐 Ruby | 📅 2026-02-24 – A jq wrapper for Ruby.

## Podcasts and presentations

* [ThePrimeTime - The BEST CLI Tool](https://www.youtube.com/watch?v=n8sOmEe2SDg)
* [Programming By Stealth](https://pbs.bartificer.net/) ([instalments](https://pbs.bartificer.net/#instalments) PBS 155 to PBS 167)

## Contribute

Please contribute! Open an issue or a PR and we’ll discuss it or merge it. If
you’re opening a PR, please ensure all formatting is ok (if you’re in a hurry
just open an issue).

## License

[![CC0](https://licensebuttons.net/p/zero/1.0/88x31.png)](https://creativecommons.org/publicdomain/zero/1.0/)

***

> _Enhansomed by [enhansome](https://github.com/enhansome) on 2026-08-22._
