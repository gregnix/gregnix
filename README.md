# gregnix

Tcl/Tk, PDF, Markdown and Cairo development.

## Projects

### Documentation suite

Pure-Tcl stack with a shared intermediate representation.
In active development; APIs may change.

**Libraries**

* [docir](https://github.com/gregnix/docir) — AST/IR spec and renderers
  (HTML, PDF, MD, nroff, SVG, canvas, tile)
* [mdstack](https://github.com/gregnix/mdstack) — Markdown parser,
  viewer, renderers
* [tcldocs-config](https://github.com/gregnix/tcldocs-config) —
  cross-app shared settings (`~/.tcldocs.rc`)
* [tcldocs-launcher](https://github.com/gregnix/tcldocs-launcher) —
  cross-app tool launcher (Tools-menu, app autodetect)

**Apps**

* [mdhelp](https://github.com/gregnix/mdhelp) — Markdown viewer/editor app
* [man-viewer](https://github.com/gregnix/man-viewer) — nroff viewer,
  CLI converters, `nroffide`
* [tcltk-glossary](https://github.com/gregnix/tcltk-glossary) —
  SQLite glossary with FTS5 search, GUI + TUI
* [cheatsheets](https://github.com/gregnix/cheatsheets) —
  cheatsheet renderer (CSD format → PDF/HTML via docir)

**Tools**

* [tcltk-manindex](https://github.com/gregnix/tcltk-manindex) —
  Tcl/Tk manpage indexer with FTS5 + auto-generated cheatsheets

### PDF

* [pdf4tcl](https://github.com/gregnix/pdf4tcl) — fork with extensions
  (encryption, PDF/A, Unicode/CID fonts)
* [pdf4tcllib](https://github.com/gregnix/pdf4tcllib) — layout,
  AcroForms, page templates
* [tclpdfium](https://github.com/gregnix/tclpdfium) — PDFium integration

### Graphics

* [tclmcairo](https://github.com/gregnix/tclmcairo) — Cairo bindings
  (PDF, SVG, 2D)

## Platforms

Linux and Windows, Tcl/Tk 8.6 and 9.x.