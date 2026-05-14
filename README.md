# gregnix

Tcl/Tk, PDF, Markdown and Cairo development.

## Projects

### Documentation suite

Pure-Tcl applications and libraries with a shared intermediate
representation. The apps interoperate — right-click in mdhelp or
man-viewer to look up a word in tcltk-glossary; settings and tool
paths are shared via `~/.tcldocs.rc`.

Pre-1.0 — refinements in progress, breaking changes possible.

**Apps**

* [mdhelp](https://github.com/gregnix/mdhelp) — Markdown viewer / editor
  with PDF export and full-text search
* [man-viewer](https://github.com/gregnix/man-viewer) — nroff viewer,
  CLI converters (n2html / n2md / n2pdf / n2svg / n2txt), and
  `nroffide` (nroff IDE with debugger)
* [tcltk-glossary](https://github.com/gregnix/tcltk-glossary) —
  SQLite-backed Tcl/Tk glossary with FTS5 search, GUI and TUI
* [cheatsheets](https://github.com/gregnix/cheatsheets) —
  cheatsheet renderer (CSD format → PDF / HTML / Markdown via docir)

**Libraries**

* [docir](https://github.com/gregnix/docir) — document intermediate
  representation and renderer family (HTML, PDF, Markdown, nroff,
  SVG, canvas, tile)
* [mdstack](https://github.com/gregnix/mdstack) — Markdown parser,
  viewer, and renderers (adapter on docir)
* [tcldocs-config](https://github.com/gregnix/tcldocs-config) —
  cross-app shared settings (`~/.tcldocs.rc`)
* [tcldocs-launcher](https://github.com/gregnix/tcldocs-launcher) —
  cross-app tool launcher (Tools menu, app autodetect)

**Tools**

* [tcltk-manindex](https://github.com/gregnix/tcltk-manindex) —
  Tcl/Tk manpage indexer with FTS5 search and auto-generated
  cheatsheets

### PDF

* [pdf4tcl](https://github.com/gregnix/pdf4tcl) — fork with extensions
  (encryption, PDF/A, Unicode / CID fonts)
* [pdf4tcllib](https://github.com/gregnix/pdf4tcllib) — layout,
  AcroForms, page templates
* [tclpdfium](https://github.com/gregnix/tclpdfium) — PDFium integration

### Graphics

* [tclmcairo](https://github.com/gregnix/tclmcairo) — Cairo bindings
  (PDF, SVG, 2D)

## Platforms

Linux and Windows, Tcl/Tk 8.6 and 9.x.
