# gregnix

Tcl/Tk, PDF, Markdown, and Cairo development — and Tcl/Tk documentation
in English and German.

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
  representation: nroff and Markdown in; HTML, PDF, Markdown, nroff,
  SVG, Tk and canvas renderers out (plus tile output for HTML, PDF and
  Markdown)
* [mdstack](https://github.com/gregnix/mdstack) — Markdown parser,
  viewer, and renderers (adapter on
  [docir](https://github.com/gregnix/docir)), plus `mdserver`, an
  HTTP/HTTPS Markdown web server
* [tcldocs-config](https://github.com/gregnix/tcldocs-config) —
  cross-app shared settings (`~/.tcldocs.rc`)
* [tcldocs-launcher](https://github.com/gregnix/tcldocs-launcher) —
  cross-app tool launcher (Tools menu, app autodetect)
* [tcldocs-search](https://github.com/gregnix/tcldocs-search) —
  cross-app search component for the documentation suite

**Tools**

* [tcltk-manindex](https://github.com/gregnix/tcltk-manindex) —
  Tcl/Tk manpage indexer with FTS5 search and auto-generated
  cheatsheets
* [bookkit](https://github.com/gregnix/bookkit) — toolkit and rulebook
  for books in the docir + mdstack + pdf4tcl format: Markdown chapters
  → PDF and HTML with numbering, table of contents, subject index and
  multilingual support

### Manuals

* [tcltk-manuals](https://github.com/gregnix/tcltk-manuals) — manual
  pages for Tcl/Tk 9.0 and 8.6 (including the C API), Tcllib, Tklib,
  Csaba Nemethi's packages (tablelist, mentry, scrollutil, wcb, tsw) and
  extensions (TDBC, Thread, [incr Tcl], BWidget, tDOM, expect, …) as
  Markdown and PDF, English original and German translation, with a
  combined PDF index; plus books on tclutils, tkutils, pdf4tcl,
  pdf4tcllib and mdserver. Unofficial collection; built with
  docir / mdstack / pdf4tcl

### OpenDocument & spreadsheets

Native OpenDocument tooling for Tcl — read / write ODF and evaluate
spreadsheet formulas without LibreOffice, validated against real
LibreOffice output.

* [odf](https://github.com/gregnix/odf) — native OpenDocument library
  (read / write ODT / ODS / ODG / ODC / ODB), pass-through-first
* [ofcalc](https://github.com/gregnix/ofcalc) — OpenFormula calculation
  engine (parser, evaluator, dependency recalc, optional `odf` adapter)
* [refcorpus](https://github.com/gregnix/refcorpus) — shared LibreOffice
  reference corpus and comparison tools for `odf` / `ofcalc`
* [tcl-peg-notes](https://github.com/gregnix/tcl-peg-notes) — PEG / tcllib
  parser docs plus PEG-in-Tcl/Tk and UNO / LibreOffice handbooks (docs)

### PDF

Writing, reading, and modifying PDFs from pure Tcl — plus a PDFium
binding where native speed or page rendering is needed. The reader and
writer keep to one rule: they never touch an existing content stream,
they overlay.

* [pdf4tcl](https://github.com/gregnix/pdf4tcl) — unofficial fork of
  [pdf4tcl](https://sourceforge.net/projects/pdf4tcl/) by Peter Spjuth,
  with extensions (Unicode / CID fonts, PDF/A, Tagged PDF and PDF/UA,
  AES-256 encryption, optional content layers, form fields with comb
  cells and date formats)
* [pdf4tcllib](https://github.com/gregnix/pdf4tcllib) — layout,
  AcroForms, page templates
* [tclpdfreader](https://github.com/gregnix/tclpdfreader) — read-only
  inspection across three backends (pure Tcl, PDFium, qpdf): page
  geometry, text, layers, attachments, encryption. None of the backends
  is required; missing ones simply narrow the answer
* [tclpdfwriter](https://github.com/gregnix/tclpdfwriter) — modify
  existing PDFs without rewriting their content: stamp, watermark,
  page operations, metadata, flatten
* [tclpdfium](https://github.com/gregnix/tclpdfium) — PDFium binding:
  text and search with rectangles, clipped and print-mode rendering,
  page objects, form fields, flatten
* [printlib](https://github.com/gregnix/printlib) — cross-platform PDF
  printing (Windows GDI / pdfium, Linux CUPS), with Brother QL label support

### Graphics

* [tclmcairo](https://github.com/gregnix/tclmcairo) — Cairo bindings
  for Tcl/Tk (PDF, SVG, PostScript, EPS, PNG)
* [tcllunasvg](https://github.com/gregnix/tcllunasvg) — lunasvg binding
  for Tcl (SVG → ARGB32 / PNG); pairs with tclmcairo via
  `image_from_argb32`
* [tkmcairo](https://github.com/gregnix/tkmcairo) — Tk widgets built
  on tclmcairo (surface, plot, imageviewer, svgview, pageview, scene,
  viewport)

### Tk widgets

* [ruledtext](https://github.com/gregnix/ruledtext) — notebook-paper
  style text widget with lines, margins, presets, and PDF export
* [tkprintcompat](https://github.com/gregnix/tkprintcompat) — Tk 8.6
  compatibility layer for the modern Tk printing API
* [tcllitehtml](https://github.com/gregnix/tcllitehtml) — HTML / CSS
  widget for Tcl/Tk

### Utility libraries

Three layers, pure Tcl: logic, widgets, and the glue between them.

* [tclutils](https://github.com/gregnix/tclutils) — general-purpose utility
  library for Tcl, no Tk (text and data formats, diagrams, ZIP / DOCX /
  XLSX / ODF, HTTP / WebDAV, diagnostics)
* [tkutils](https://github.com/gregnix/tkutils) — utility and widget helpers
  for Tk
* [ctrlutils](https://github.com/gregnix/ctrlutils) — controllers that
  connect tkutils widgets to tclutils providers (file operations,
  monitoring, undo, sync, filters)
* [tical](https://github.com/gregnix/tical) — calendar library: views,
  events, rendering to canvas and PDF, iCalendar import and export

### Build

* [tea-cxx](https://github.com/gregnix/tea-cxx) — experiment: building
  C++ Tcl extensions with TEA

## Platforms

Linux and Windows, Tcl/Tk 8.6 and 9.x.
