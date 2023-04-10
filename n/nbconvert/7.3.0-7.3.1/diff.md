# Comparing `tmp/nbconvert-7.3.0.tar.gz` & `tmp/nbconvert-7.3.1.tar.gz`

## Comparing `nbconvert-7.3.0.tar` & `nbconvert-7.3.1.tar`

### file list

```diff
@@ -1,276 +1,276 @@
--rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.git-blame-ignore-revs
--rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.mailmap
--rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.pre-commit-config.yaml
--rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.prettierignore
--rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.readthedocs.yaml
--rw-r--r--   0        0        0    69337 2020-02-02 00:00:00.000000 nbconvert-7.3.0/CHANGELOG.md
--rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.3.0/CONTRIBUTING.md
--rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.3.0/RELEASE.md
--rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.3.0/check_requirements.py
--rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nbconvert-7.3.0/codecov.yml
--rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/dependabot.yml
--rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/ISSUE_TEMPLATE/bug_report.md
--rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/ISSUE_TEMPLATE/feature_request.md
--rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/ISSUE_TEMPLATE/question.md
--rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/workflows/docs.yml
--rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/workflows/enforce-label.yml
--rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/workflows/prep-release.yml
--rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/workflows/publish-release.yml
--rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.github/workflows/tests.yml
--rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/Makefile
--rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/README.md
--rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/autogen_config.py
--rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/make.bat
--rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/make_html.py
--rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/quiz_notebook.py
--rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/media/image1.png
--rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/media/image2.png
--rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
--rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
--rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
--rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/architecture.rst
--rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/conf.py
--rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/customizing.rst
--rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/dejavu.rst
--rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/development_release.rst
--rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/execute_api.rst
--rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/external_exporters.rst
--rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/highlighting.rst
--rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/index.rst
--rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/install.rst
--rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/latex_citations.rst
--rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/nbconvert_library.ipynb
--rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/need_help.rst
--rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/removing_cells.rst
--rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/usage.rst
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/_static/empty.txt
--rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/_static/exporter_inheritance.png
--rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/_static/preprocessor_inheritance.png
--rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/_static/writer_inheritance.png
--rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/exporters.rst
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/filters.rst
--rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/index.rst
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/nbconvertapp.rst
--rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/postprocessors.rst
--rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/preprocessors.rst
--rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.3.0/docs/source/api/writers.rst
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/__init__.py
--rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/__main__.py
--rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/_version.py
--rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/conftest.py
--rwxr-xr-x   0        0        0    24756 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/nbconvertapp.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/py.typed
--rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/__init__.py
--rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/asciidoc.py
--rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/base.py
--rw-r--r--   0        0        0    12635 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/exporter.py
--rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/html.py
--rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/latex.py
--rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/markdown.py
--rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/notebook.py
--rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/pdf.py
--rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/python.py
--rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/qt_exporter.py
--rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/qt_screenshot.py
--rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/qtpdf.py
--rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/qtpng.py
--rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/rst.py
--rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/script.py
--rw-r--r--   0        0        0     6434 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/slides.py
--rw-r--r--   0        0        0    26829 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/templateexporter.py
--rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/webpdf.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/__init__.py
--rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/base.py
--rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/cheese.py
--rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_asciidoc.py
--rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_export.py
--rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_exporter.py
--rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_html.py
--rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_latex.py
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_markdown.py
--rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_notebook.py
--rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_pdf.py
--rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_python.py
--rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_qtpdf.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_qtpng.py
--rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_rst.py
--rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_script.py
--rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_slides.py
--rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_templateexporter.py
--rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/test_webpdf.py
--rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/attachment.ipynb
--rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/lablike.html.j2
--rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/notebook3.ipynb
--rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/notebook_inject.ipynb
--rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/pngmetadata.ipynb
--rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb
--rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/rawtest.ipynb
--rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/exporters/tests/files/svg.ipynb
--rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/__init__.py
--rw-r--r--   0        0        0     8020 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/ansi.py
--rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/citation.py
--rw-r--r--   0        0        0     1571 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/datatypefilter.py
--rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/filter_links.py
--rw-r--r--   0        0        0     6073 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/highlight.py
--rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/latex.py
--rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/markdown.py
--rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/markdown_mistune.py
--rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/metadata.py
--rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/pandoc.py
--rw-r--r--   0        0        0     7656 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/strings.py
--rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/svg_constants.py
--rw-r--r--   0        0        0     2835 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/widgetsdatatypefilter.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/__init__.py
--rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_ansi.py
--rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_citation.py
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_datatypefilter.py
--rw-r--r--   0        0        0     2788 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_highlight.py
--rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_latex.py
--rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_markdown.py
--rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_metadata.py
--rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/filters/tests/test_strings.py
--rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/postprocessors/__init__.py
--rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/postprocessors/base.py
--rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/postprocessors/serve.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/postprocessors/tests/__init__.py
--rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/postprocessors/tests/test_serve.py
--rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/__init__.py
--rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/base.py
--rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/clearmetadata.py
--rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/clearoutput.py
--rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/coalescestreams.py
--rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/convertfigures.py
--rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/csshtmlheader.py
--rw-r--r--   0        0        0     4597 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/execute.py
--rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/extractoutput.py
--rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/highlightmagics.py
--rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/latex.py
--rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/regexremove.py
--rw-r--r--   0        0        0     5317 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/sanitize.py
--rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/svg2pdf.py
--rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tagremove.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/__init__.py
--rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/base.py
--rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/fake_kernelmanager.py
--rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_clearmetadata.py
--rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_clearoutput.py
--rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_coalescestreams.py
--rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_csshtmlheader.py
--rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_execute.py
--rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_extractoutput.py
--rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_highlightmagics.py
--rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_latex.py
--rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_regexremove.py
--rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_sanitize.py
--rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_svg2pdf.py
--rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/test_tagremove.py
--rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
--rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/resources/__init__.py
--rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/templates/README.md
--rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/templates/skeleton/Makefile
--rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/templates/skeleton/README.md
--rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/README.md
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/__init__.py
--rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/base.py
--rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/fake_exporters.py
--rw-r--r--   0        0        0    28677 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/test_nbconvertapp.py
--rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/utils.py
--rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/exporter_entrypoint/eptest.py
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/Unexecuted_widget.ipynb
--rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb
--rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/Widget_List.ipynb
--rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/containerized_deployments.jpeg
--rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/hello.py
--rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/issue1849_svg.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/jupyter_nbconvert_config.py
--rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/latex-linked-image.ipynb
--rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/markdown_display_priority.ipynb
--rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook1.ipynb
--rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook2.ipynb
--rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook3_with_errors.ipynb
--rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook4_jpeg.ipynb
--rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook5_embed_images.ipynb
--rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook_jl.ipynb
--rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/notebook_tags.ipynb
--rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/override.py
--rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/tests/files/testimage.png
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/__init__.py
--rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/_contextlib_chdir.py
--rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/base.py
--rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/exceptions.py
--rw-r--r--   0        0        0     3704 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/io.py
--rw-r--r--   0        0        0      216 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/lexers.py
--rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/pandoc.py
--rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/text.py
--rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/version.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/tests/__init__.py
--rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/tests/test_io.py
--rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/tests/test_pandoc.py
--rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/utils/tests/test_version.py
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/__init__.py
--rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/base.py
--rw-r--r--   0        0        0     1520 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/debug.py
--rw-r--r--   0        0        0     4995 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/files.py
--rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/stdout.py
--rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/tests/__init__.py
--rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/tests/test_debug.py
--rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/tests/test_files.py
--rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.3.0/nbconvert/writers/tests/test_stdout.py
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/asciidoc/conf.json
--rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/asciidoc/index.asciidoc.j2
--rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/base/cell_id_anchor.j2
--rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/base/celltags.j2
--rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/base/display_priority.j2
--rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/base/jupyter_widgets.html.j2
--rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/base/mathjax.html.j2
--rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/base/null.j2
--rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/basic/conf.json
--rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/basic/index.html.j2
--rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/classic/base.html.j2
--rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/classic/conf.json
--rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/classic/index.html.j2
--rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/classic/static/style.css
--rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/compatibility/display_priority.tpl
--rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/compatibility/full.tpl
--rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/lab/base.html.j2
--rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/lab/conf.json
--rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/lab/index.html.j2
--rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/lab/static/index.css
--rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/lab/static/theme-dark.css
--rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/lab/static/theme-light.css
--rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/base.tex.j2
--rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/conf.json
--rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/display_priority.j2
--rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/document_contents.tex.j2
--rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/index.tex.j2
--rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/null.j2
--rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/report.tex.j2
--rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/style_bw_ipython.tex.j2
--rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/style_bw_python.tex.j2
--rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/style_ipython.tex.j2
--rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/style_jupyter.tex.j2
--rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/latex/style_python.tex.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/markdown/conf.json
--rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/markdown/index.md.j2
--rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/python/conf.json
--rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/python/index.py.j2
--rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/reveal/base.html.j2
--rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/reveal/cellslidedata.j2
--rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/reveal/conf.json
--rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/reveal/index.html.j2
--rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/reveal/static/custom_reveal.css
--rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/rst/conf.json
--rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/rst/index.rst.j2
--rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/script/conf.json
--rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/script/script.j2
--rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/webpdf/conf.json
--rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.3.0/share/templates/webpdf/index.pdf.j2
--rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.3.0/.gitignore
--rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.3.0/LICENSE
--rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 nbconvert-7.3.0/README.md
--rw-r--r--   0        0        0     2650 2020-02-02 00:00:00.000000 nbconvert-7.3.0/hatch_build.py
--rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 nbconvert-7.3.0/pyproject.toml
--rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 nbconvert-7.3.0/PKG-INFO
+-rw-r--r--   0        0        0       71 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.git-blame-ignore-revs
+-rw-r--r--   0        0        0    10806 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.mailmap
+-rw-r--r--   0        0        0     1035 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.pre-commit-config.yaml
+-rw-r--r--   0        0        0       29 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.prettierignore
+-rw-r--r--   0        0        0      345 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.readthedocs.yaml
+-rw-r--r--   0        0        0    70125 2020-02-02 00:00:00.000000 nbconvert-7.3.1/CHANGELOG.md
+-rw-r--r--   0        0        0     2390 2020-02-02 00:00:00.000000 nbconvert-7.3.1/CONTRIBUTING.md
+-rw-r--r--   0        0        0     1615 2020-02-02 00:00:00.000000 nbconvert-7.3.1/RELEASE.md
+-rw-r--r--   0        0        0      729 2020-02-02 00:00:00.000000 nbconvert-7.3.1/check_requirements.py
+-rw-r--r--   0        0        0      135 2020-02-02 00:00:00.000000 nbconvert-7.3.1/codecov.yml
+-rw-r--r--   0        0        0      219 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/dependabot.yml
+-rw-r--r--   0        0        0      504 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/ISSUE_TEMPLATE/bug_report.md
+-rw-r--r--   0        0        0      365 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/ISSUE_TEMPLATE/feature_request.md
+-rw-r--r--   0        0        0      262 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/ISSUE_TEMPLATE/question.md
+-rw-r--r--   0        0        0     1510 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/docs.yml
+-rw-r--r--   0        0        0      320 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/enforce-label.yml
+-rw-r--r--   0        0        0     1455 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/prep-release.yml
+-rw-r--r--   0        0        0     1854 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/publish-release.yml
+-rw-r--r--   0        0        0     4742 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.github/workflows/tests.yml
+-rw-r--r--   0        0        0     7460 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/Makefile
+-rw-r--r--   0        0        0     1506 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/README.md
+-rw-r--r--   0        0        0     2245 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/autogen_config.py
+-rw-r--r--   0        0        0     7259 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/make.bat
+-rw-r--r--   0        0        0      739 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/make_html.py
+-rw-r--r--   0        0        0     2173 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/quiz_notebook.py
+-rw-r--r--   0        0        0    36829 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/media/image1.png
+-rw-r--r--   0        0        0   176383 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/media/image2.png
+-rw-r--r--   0        0        0       74 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/conf.json
+-rw-r--r--   0        0        0     3322 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2
+-rw-r--r--   0        0        0   266255 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css
+-rw-r--r--   0        0        0     8651 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/architecture.rst
+-rw-r--r--   0        0        0    10812 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/conf.py
+-rw-r--r--   0        0        0     6750 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/customizing.rst
+-rw-r--r--   0        0        0     1254 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/dejavu.rst
+-rw-r--r--   0        0        0     3911 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/development_release.rst
+-rw-r--r--   0        0        0     7875 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/execute_api.rst
+-rw-r--r--   0        0        0     8330 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/external_exporters.rst
+-rw-r--r--   0        0        0     1910 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/highlighting.rst
+-rw-r--r--   0        0        0     2037 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/index.rst
+-rw-r--r--   0        0        0     3425 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/install.rst
+-rw-r--r--   0        0        0      590 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/latex_citations.rst
+-rw-r--r--   0        0        0    18384 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/nbconvert_library.ipynb
+-rw-r--r--   0        0        0     1129 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/need_help.rst
+-rw-r--r--   0        0        0     3519 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/removing_cells.rst
+-rw-r--r--   0        0        0    11750 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/usage.rst
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/empty.txt
+-rw-r--r--   0        0        0    36971 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/exporter_inheritance.png
+-rw-r--r--   0        0        0    65726 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/preprocessor_inheritance.png
+-rw-r--r--   0        0        0     8182 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/_static/writer_inheritance.png
+-rw-r--r--   0        0        0     1237 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/exporters.rst
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/filters.rst
+-rw-r--r--   0        0        0      227 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/index.rst
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/nbconvertapp.rst
+-rw-r--r--   0        0        0      355 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/postprocessors.rst
+-rw-r--r--   0        0        0     1151 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/preprocessors.rst
+-rw-r--r--   0        0        0      354 2020-02-02 00:00:00.000000 nbconvert-7.3.1/docs/source/api/writers.rst
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/__init__.py
+-rw-r--r--   0        0        0       72 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/__main__.py
+-rw-r--r--   0        0        0      498 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/_version.py
+-rw-r--r--   0        0        0      165 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/conftest.py
+-rwxr-xr-x   0        0        0    24764 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/nbconvertapp.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/py.typed
+-rw-r--r--   0        0        0      618 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/__init__.py
+-rw-r--r--   0        0        0     1445 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/asciidoc.py
+-rw-r--r--   0        0        0     4954 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/base.py
+-rw-r--r--   0        0        0    12643 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/exporter.py
+-rw-r--r--   0        0        0    11185 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/html.py
+-rw-r--r--   0        0        0     3007 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/latex.py
+-rw-r--r--   0        0        0     1415 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/markdown.py
+-rw-r--r--   0        0        0     1423 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/notebook.py
+-rw-r--r--   0        0        0     7852 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/pdf.py
+-rw-r--r--   0        0        0      675 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/python.py
+-rw-r--r--   0        0        0     2126 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qt_exporter.py
+-rw-r--r--   0        0        0     3157 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qt_screenshot.py
+-rw-r--r--   0        0        0      789 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qtpdf.py
+-rw-r--r--   0        0        0      487 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/qtpng.py
+-rw-r--r--   0        0        0      904 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/rst.py
+-rw-r--r--   0        0        0     3128 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/script.py
+-rw-r--r--   0        0        0     6465 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/slides.py
+-rw-r--r--   0        0        0    26957 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/templateexporter.py
+-rw-r--r--   0        0        0     6069 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/webpdf.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/__init__.py
+-rw-r--r--   0        0        0     1286 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/base.py
+-rw-r--r--   0        0        0     1458 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/cheese.py
+-rw-r--r--   0        0        0     2220 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_asciidoc.py
+-rw-r--r--   0        0        0     3369 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_export.py
+-rw-r--r--   0        0        0     3415 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_exporter.py
+-rw-r--r--   0        0        0     7891 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_html.py
+-rw-r--r--   0        0        0     6707 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_latex.py
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_markdown.py
+-rw-r--r--   0        0        0     1360 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_notebook.py
+-rw-r--r--   0        0        0     1361 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_pdf.py
+-rw-r--r--   0        0        0      830 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_python.py
+-rw-r--r--   0        0        0      704 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpdf.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpng.py
+-rw-r--r--   0        0        0     2121 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_rst.py
+-rw-r--r--   0        0        0     2371 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_script.py
+-rw-r--r--   0        0        0     3013 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_slides.py
+-rw-r--r--   0        0        0    27769 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_templateexporter.py
+-rw-r--r--   0        0        0     1712 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/test_webpdf.py
+-rw-r--r--   0        0        0    45585 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/attachment.ipynb
+-rw-r--r--   0        0        0       98 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/lablike.html.j2
+-rw-r--r--   0        0        0    10437 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0      997 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook3.ipynb
+-rw-r--r--   0        0        0     6056 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook_inject.ipynb
+-rw-r--r--   0        0        0    16782 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/pngmetadata.ipynb
+-rw-r--r--   0        0        0     1356 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/prompt_numbers.ipynb
+-rw-r--r--   0        0        0     1213 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/rawtest.ipynb
+-rw-r--r--   0        0        0    19943 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/exporters/tests/files/svg.ipynb
+-rw-r--r--   0        0        0      254 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/__init__.py
+-rw-r--r--   0        0        0     8060 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/ansi.py
+-rw-r--r--   0        0        0     3667 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/citation.py
+-rw-r--r--   0        0        0     1598 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/datatypefilter.py
+-rw-r--r--   0        0        0     1547 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/filter_links.py
+-rw-r--r--   0        0        0     6169 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/highlight.py
+-rw-r--r--   0        0        0     1819 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/latex.py
+-rw-r--r--   0        0        0     2849 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/markdown.py
+-rw-r--r--   0        0        0     9888 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/markdown_mistune.py
+-rw-r--r--   0        0        0      477 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/metadata.py
+-rw-r--r--   0        0        0      736 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/pandoc.py
+-rw-r--r--   0        0        0     7683 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/strings.py
+-rw-r--r--   0        0        0     3414 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/svg_constants.py
+-rw-r--r--   0        0        0     2862 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/widgetsdatatypefilter.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/__init__.py
+-rw-r--r--   0        0        0     3960 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_ansi.py
+-rw-r--r--   0        0        0     4407 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_citation.py
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_datatypefilter.py
+-rw-r--r--   0        0        0     2796 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_highlight.py
+-rw-r--r--   0        0        0     1658 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_latex.py
+-rw-r--r--   0        0        0     8534 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_markdown.py
+-rw-r--r--   0        0        0      617 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_metadata.py
+-rw-r--r--   0        0        0     7444 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/filters/tests/test_strings.py
+-rw-r--r--   0        0        0      151 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/__init__.py
+-rw-r--r--   0        0        0     1154 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/base.py
+-rw-r--r--   0        0        0     4272 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/serve.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/tests/__init__.py
+-rw-r--r--   0        0        0      649 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/postprocessors/tests/test_serve.py
+-rw-r--r--   0        0        0      769 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/__init__.py
+-rw-r--r--   0        0        0     2842 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/base.py
+-rw-r--r--   0        0        0     3776 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/clearmetadata.py
+-rw-r--r--   0        0        0      930 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/clearoutput.py
+-rw-r--r--   0        0        0     2257 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/coalescestreams.py
+-rw-r--r--   0        0        0     1540 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/convertfigures.py
+-rw-r--r--   0        0        0     3268 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/csshtmlheader.py
+-rw-r--r--   0        0        0     4558 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/execute.py
+-rw-r--r--   0        0        0     6462 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/extractoutput.py
+-rw-r--r--   0        0        0     3216 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/highlightmagics.py
+-rw-r--r--   0        0        0     2736 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/latex.py
+-rw-r--r--   0        0        0     2481 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/regexremove.py
+-rw-r--r--   0        0        0     5369 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/sanitize.py
+-rw-r--r--   0        0        0     5537 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/svg2pdf.py
+-rw-r--r--   0        0        0     4511 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tagremove.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/__init__.py
+-rw-r--r--   0        0        0     2070 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/base.py
+-rw-r--r--   0        0        0      805 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/fake_kernelmanager.py
+-rw-r--r--   0        0        0     5145 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearmetadata.py
+-rw-r--r--   0        0        0     1894 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearoutput.py
+-rw-r--r--   0        0        0     2891 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_coalescestreams.py
+-rw-r--r--   0        0        0     1576 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_csshtmlheader.py
+-rw-r--r--   0        0        0     3793 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_execute.py
+-rw-r--r--   0        0        0     3196 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_extractoutput.py
+-rw-r--r--   0        0        0     1718 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_highlightmagics.py
+-rw-r--r--   0        0        0     1750 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_latex.py
+-rw-r--r--   0        0        0     2475 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_regexremove.py
+-rw-r--r--   0        0        0     6237 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_sanitize.py
+-rw-r--r--   0        0        0     3350 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_svg2pdf.py
+-rw-r--r--   0        0        0     2872 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/test_tagremove.py
+-rw-r--r--   0        0        0      357 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/files/HelloWorld.ipynb
+-rw-r--r--   0        0        0      820 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/resources/__init__.py
+-rw-r--r--   0        0        0      307 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/templates/README.md
+-rw-r--r--   0        0        0      682 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/templates/skeleton/Makefile
+-rw-r--r--   0        0        0      510 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/templates/skeleton/README.md
+-rw-r--r--   0        0        0      104 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/README.md
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/__init__.py
+-rw-r--r--   0        0        0     6251 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/base.py
+-rw-r--r--   0        0        0      543 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/fake_exporters.py
+-rw-r--r--   0        0        0    28677 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/test_nbconvertapp.py
+-rw-r--r--   0        0        0      332 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/utils.py
+-rw-r--r--   0        0        0      232 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/exporter_entrypoint/eptest.py
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/exporter_entrypoint/eptest-0.1.dist-info/entry_points.txt
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget.ipynb
+-rw-r--r--   0        0        0      988 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget_2.ipynb
+-rw-r--r--   0        0        0    96479 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/Widget_List.ipynb
+-rw-r--r--   0        0        0    12779 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/containerized_deployments.jpeg
+-rw-r--r--   0        0        0      234 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/hello.py
+-rw-r--r--   0        0        0    18524 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/issue1849_svg.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/jupyter_nbconvert_config.py
+-rw-r--r--   0        0        0      541 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/latex-linked-image.ipynb
+-rw-r--r--   0        0        0     8691 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/markdown_display_priority.ipynb
+-rw-r--r--   0        0        0     5670 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook1.ipynb
+-rw-r--r--   0        0        0   125459 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook2.ipynb
+-rw-r--r--   0        0        0     1318 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook3_with_errors.ipynb
+-rw-r--r--   0        0        0    18657 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook4_jpeg.ipynb
+-rw-r--r--   0        0        0      938 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook5_embed_images.ipynb
+-rw-r--r--   0        0        0      450 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook_jl.ipynb
+-rw-r--r--   0        0        0     1618 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/notebook_tags.ipynb
+-rw-r--r--   0        0        0      208 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/override.py
+-rw-r--r--   0        0        0     1923 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/tests/files/testimage.png
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/__init__.py
+-rw-r--r--   0        0        0      593 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/_contextlib_chdir.py
+-rw-r--r--   0        0        0     1088 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/base.py
+-rw-r--r--   0        0        0      690 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/exceptions.py
+-rw-r--r--   0        0        0     3712 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/io.py
+-rw-r--r--   0        0        0      230 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/lexers.py
+-rw-r--r--   0        0        0     4462 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/pandoc.py
+-rw-r--r--   0        0        0     1091 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/text.py
+-rw-r--r--   0        0        0      951 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/version.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/__init__.py
+-rw-r--r--   0        0        0     1001 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/test_io.py
+-rw-r--r--   0        0        0     2919 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/test_pandoc.py
+-rw-r--r--   0        0        0      426 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/utils/tests/test_version.py
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/__init__.py
+-rw-r--r--   0        0        0     1187 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/base.py
+-rw-r--r--   0        0        0     1528 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/debug.py
+-rw-r--r--   0        0        0     5003 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/files.py
+-rw-r--r--   0        0        0      514 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/stdout.py
+-rw-r--r--   0        0        0        0 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/__init__.py
+-rw-r--r--   0        0        0     1529 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/test_debug.py
+-rw-r--r--   0        0        0    10268 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/test_files.py
+-rw-r--r--   0        0        0     1367 2020-02-02 00:00:00.000000 nbconvert-7.3.1/nbconvert/writers/tests/test_stdout.py
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/asciidoc/conf.json
+-rw-r--r--   0        0        0     2298 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/asciidoc/index.asciidoc.j2
+-rw-r--r--   0        0        0      160 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/cell_id_anchor.j2
+-rw-r--r--   0        0        0      231 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/celltags.j2
+-rw-r--r--   0        0        0     1442 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/display_priority.j2
+-rw-r--r--   0        0        0     1250 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/jupyter_widgets.html.j2
+-rw-r--r--   0        0        0     1188 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/mathjax.html.j2
+-rw-r--r--   0        0        0     6265 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/base/null.j2
+-rw-r--r--   0        0        0       77 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/basic/conf.json
+-rw-r--r--   0        0        0       39 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/basic/index.html.j2
+-rw-r--r--   0        0        0     8261 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/base.html.j2
+-rw-r--r--   0        0        0      243 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/conf.json
+-rw-r--r--   0        0        0     2370 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/index.html.j2
+-rw-r--r--   0        0        0   265101 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/classic/static/style.css
+-rw-r--r--   0        0        0      133 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/compatibility/display_priority.tpl
+-rw-r--r--   0        0        0      124 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/compatibility/full.tpl
+-rw-r--r--   0        0        0     9816 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/base.html.j2
+-rw-r--r--   0        0        0      217 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/conf.json
+-rw-r--r--   0        0        0     4002 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/index.html.j2
+-rw-r--r--   0        0        0   581722 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/static/index.css
+-rw-r--r--   0        0        0    16733 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/static/theme-dark.css
+-rw-r--r--   0        0        0    15637 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/lab/static/theme-light.css
+-rw-r--r--   0        0        0     9662 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/base.tex.j2
+-rw-r--r--   0        0        0      126 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/conf.json
+-rw-r--r--   0        0        0     1643 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/display_priority.j2
+-rw-r--r--   0        0        0     2746 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/document_contents.tex.j2
+-rw-r--r--   0        0        0      496 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/index.tex.j2
+-rw-r--r--   0        0        0     5544 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/null.j2
+-rw-r--r--   0        0        0      909 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/report.tex.j2
+-rw-r--r--   0        0        0     1989 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_bw_ipython.tex.j2
+-rw-r--r--   0        0        0      479 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_bw_python.tex.j2
+-rw-r--r--   0        0        0     2587 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_ipython.tex.j2
+-rw-r--r--   0        0        0     8233 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_jupyter.tex.j2
+-rw-r--r--   0        0        0      794 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/latex/style_python.tex.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/markdown/conf.json
+-rw-r--r--   0        0        0     2028 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/markdown/index.md.j2
+-rw-r--r--   0        0        0       78 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/python/conf.json
+-rw-r--r--   0        0        0      472 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/python/index.py.j2
+-rw-r--r--   0        0        0      872 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/base.html.j2
+-rw-r--r--   0        0        0      410 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/cellslidedata.j2
+-rw-r--r--   0        0        0      337 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/conf.json
+-rw-r--r--   0        0        0     5328 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/index.html.j2
+-rw-r--r--   0        0        0     2374 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/reveal/static/custom_reveal.css
+-rw-r--r--   0        0        0       86 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/rst/conf.json
+-rw-r--r--   0        0        0     2838 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/rst/index.rst.j2
+-rw-r--r--   0        0        0       75 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/script/conf.json
+-rw-r--r--   0        0        0       84 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/script/script.j2
+-rw-r--r--   0        0        0       79 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/webpdf/conf.json
+-rw-r--r--   0        0        0       36 2020-02-02 00:00:00.000000 nbconvert-7.3.1/share/templates/webpdf/index.pdf.j2
+-rw-r--r--   0        0        0      774 2020-02-02 00:00:00.000000 nbconvert-7.3.1/.gitignore
+-rw-r--r--   0        0        0     1588 2020-02-02 00:00:00.000000 nbconvert-7.3.1/LICENSE
+-rw-r--r--   0        0        0     4119 2020-02-02 00:00:00.000000 nbconvert-7.3.1/README.md
+-rw-r--r--   0        0        0     2658 2020-02-02 00:00:00.000000 nbconvert-7.3.1/hatch_build.py
+-rw-r--r--   0        0        0     7188 2020-02-02 00:00:00.000000 nbconvert-7.3.1/pyproject.toml
+-rw-r--r--   0        0        0     8055 2020-02-02 00:00:00.000000 nbconvert-7.3.1/PKG-INFO
```

### Comparing `nbconvert-7.3.0/.mailmap` & `nbconvert-7.3.1/.mailmap`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/.pre-commit-config.yaml` & `nbconvert-7.3.1/.pre-commit-config.yaml`

 * *Files 2% similar despite different names*

```diff
@@ -15,28 +15,28 @@
       - id: check-json
       - id: check-toml
       - id: check-yaml
       - id: end-of-file-fixer
       - id: trailing-whitespace
 
   - repo: https://github.com/python-jsonschema/check-jsonschema
-    rev: 0.21.0
+    rev: 0.22.0
     hooks:
       - id: check-github-workflows
 
   - repo: https://github.com/executablebooks/mdformat
     rev: 0.7.16
     hooks:
       - id: mdformat
         additional_dependencies:
           [mdformat-gfm, mdformat-frontmatter, mdformat-footnote]
 
   - repo: https://github.com/psf/black
-    rev: 23.1.0
+    rev: 23.3.0
     hooks:
       - id: black
 
   - repo: https://github.com/charliermarsh/ruff-pre-commit
-    rev: v0.0.254
+    rev: v0.0.260
     hooks:
       - id: ruff
         args: ["--fix"]
```

### Comparing `nbconvert-7.3.0/CHANGELOG.md` & `nbconvert-7.3.1/CHANGELOG.md`

 * *Files 1% similar despite different names*

```diff
@@ -1,11 +1,29 @@
 # Changes in nbconvert
 
 <!-- <START NEW CHANGELOG ENTRY> -->
 
+## 7.3.1
+
+([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.3.0...3860152ecea3d9833540eebe279ff603b3d47cea))
+
+### Bugs fixed
+
+- Remove overwriting of default KernelManager [#1972](https://github.com/jupyter/nbconvert/pull/1972) ([@tuncbkose](https://github.com/tuncbkose))
+
+### Maintenance and upkeep improvements
+
+### Contributors to this release
+
+([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-04-03&to=2023-04-10&type=c))
+
+[@pre-commit-ci](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Apre-commit-ci+updated%3A2023-04-03..2023-04-10&type=Issues) | [@tuncbkose](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Atuncbkose+updated%3A2023-04-03..2023-04-10&type=Issues)
+
+<!-- <END NEW CHANGELOG ENTRY> -->
+
 ## 7.3.0
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.2.10...056dc4ecc8f9f3e9249f0dbddf1221c65228b961))
 
 ### Enhancements made
 
 - Allow pattern in output_base [#1967](https://github.com/jupyter/nbconvert/pull/1967) ([@JeppeKlitgaard](https://github.com/JeppeKlitgaard))
@@ -19,16 +37,14 @@
 
 ### Contributors to this release
 
 ([GitHub contributors page for this release](https://github.com/jupyter/nbconvert/graphs/contributors?from=2023-03-14&to=2023-04-03&type=c))
 
 [@achimgaedke](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Aachimgaedke+updated%3A2023-03-14..2023-04-03&type=Issues) | [@blink1073](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3Ablink1073+updated%3A2023-03-14..2023-04-03&type=Issues) | [@Carreau](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3ACarreau+updated%3A2023-03-14..2023-04-03&type=Issues) | [@JeppeKlitgaard](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3AJeppeKlitgaard+updated%3A2023-03-14..2023-04-03&type=Issues) | [@martinRenou](https://github.com/search?q=repo%3Ajupyter%2Fnbconvert+involves%3AmartinRenou+updated%3A2023-03-14..2023-04-03&type=Issues)
 
-<!-- <END NEW CHANGELOG ENTRY> -->
-
 ## 7.2.10
 
 ([Full Changelog](https://github.com/jupyter/nbconvert/compare/v7.2.9...acf41acf6d83cb725f3a2c48686c828eff7b24d8))
 
 ### Enhancements made
 
 - Add cell-id anchor for cell identification [#1897](https://github.com/jupyter/nbconvert/pull/1897) ([@krassowski](https://github.com/krassowski))
```

### Comparing `nbconvert-7.3.0/CONTRIBUTING.md` & `nbconvert-7.3.1/CONTRIBUTING.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/RELEASE.md` & `nbconvert-7.3.1/RELEASE.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/check_requirements.py` & `nbconvert-7.3.1/check_requirements.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/.github/workflows/docs.yml` & `nbconvert-7.3.1/.github/workflows/docs.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/.github/workflows/prep-release.yml` & `nbconvert-7.3.1/.github/workflows/prep-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/.github/workflows/publish-release.yml` & `nbconvert-7.3.1/.github/workflows/publish-release.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/.github/workflows/tests.yml` & `nbconvert-7.3.1/.github/workflows/tests.yml`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/Makefile` & `nbconvert-7.3.1/docs/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/README.md` & `nbconvert-7.3.1/docs/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/autogen_config.py` & `nbconvert-7.3.1/docs/autogen_config.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/make.bat` & `nbconvert-7.3.1/docs/make.bat`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/api_examples/template_path/make_html.py` & `nbconvert-7.3.1/docs/api_examples/template_path/make_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/api_examples/template_path/quiz_notebook.py` & `nbconvert-7.3.1/docs/api_examples/template_path/quiz_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/api_examples/template_path/media/image1.png` & `nbconvert-7.3.1/docs/api_examples/template_path/media/image1.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/api_examples/template_path/media/image2.png` & `nbconvert-7.3.1/docs/api_examples/template_path/media/image2.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2` & `nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css` & `nbconvert-7.3.1/docs/api_examples/template_path/project_templates/nbconvert/templates/classic_clone/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/architecture.rst` & `nbconvert-7.3.1/docs/source/architecture.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/conf.py` & `nbconvert-7.3.1/docs/source/conf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/customizing.rst` & `nbconvert-7.3.1/docs/source/customizing.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/dejavu.rst` & `nbconvert-7.3.1/docs/source/dejavu.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/development_release.rst` & `nbconvert-7.3.1/docs/source/development_release.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/execute_api.rst` & `nbconvert-7.3.1/docs/source/execute_api.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/external_exporters.rst` & `nbconvert-7.3.1/docs/source/external_exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/highlighting.rst` & `nbconvert-7.3.1/docs/source/highlighting.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/index.rst` & `nbconvert-7.3.1/docs/source/index.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/install.rst` & `nbconvert-7.3.1/docs/source/install.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/latex_citations.rst` & `nbconvert-7.3.1/docs/source/latex_citations.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/nbconvert_library.ipynb` & `nbconvert-7.3.1/docs/source/nbconvert_library.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/need_help.rst` & `nbconvert-7.3.1/docs/source/need_help.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/removing_cells.rst` & `nbconvert-7.3.1/docs/source/removing_cells.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/usage.rst` & `nbconvert-7.3.1/docs/source/usage.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/_static/exporter_inheritance.png` & `nbconvert-7.3.1/docs/source/_static/exporter_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/_static/preprocessor_inheritance.png` & `nbconvert-7.3.1/docs/source/_static/preprocessor_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/_static/writer_inheritance.png` & `nbconvert-7.3.1/docs/source/_static/writer_inheritance.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/api/exporters.rst` & `nbconvert-7.3.1/docs/source/api/exporters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/api/filters.rst` & `nbconvert-7.3.1/docs/source/api/filters.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/docs/source/api/preprocessors.rst` & `nbconvert-7.3.1/docs/source/api/preprocessors.rst`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/nbconvertapp.py` & `nbconvert-7.3.1/nbconvert/nbconvertapp.py`

 * *Files 0% similar despite different names*

```diff
@@ -395,15 +395,15 @@
                     filenames.append(filename)
         self.notebooks = filenames
 
     def init_writer(self):
         """Initialize the writer (which is stateless)"""
         self._writer_class_changed({"new": self.writer_class})
         self.writer = self.writer_factory(parent=self)
-        if hasattr(self.writer, "build_directory") and self.writer.build_directory != "":
+        if hasattr(self.writer, "build_directory") and self.writer.build_directory != "":  # noqa
             self.use_output_suffix = False
 
     def init_postprocessor(self):
         """Initialize the postprocessor (which is stateless)"""
         self._postprocessor_class_changed({"new": self.postprocessor_class})
         if self.postprocessor_factory:
             self.postprocessor = self.postprocessor_factory(parent=self)
```

### Comparing `nbconvert-7.3.0/nbconvert/exporters/__init__.py` & `nbconvert-7.3.1/nbconvert/exporters/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/asciidoc.py` & `nbconvert-7.3.1/nbconvert/exporters/asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/base.py` & `nbconvert-7.3.1/nbconvert/exporters/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/exporter.py` & `nbconvert-7.3.1/nbconvert/exporters/exporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -175,15 +175,15 @@
         `**kw`
             Ignored
 
         """
         # Pull the metadata from the filesystem.
         if resources is None:
             resources = ResourcesDict()
-        if "metadata" not in resources or resources["metadata"] == "":
+        if "metadata" not in resources or resources["metadata"] == "":  # noqa
             resources["metadata"] = ResourcesDict()
         path, basename = os.path.split(filename)
         notebook_name = os.path.splitext(basename)[0]
         resources["metadata"]["name"] = notebook_name
         resources["metadata"]["path"] = path
 
         modified_date = datetime.datetime.fromtimestamp(
```

### Comparing `nbconvert-7.3.0/nbconvert/exporters/html.py` & `nbconvert-7.3.1/nbconvert/exporters/html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/latex.py` & `nbconvert-7.3.1/nbconvert/exporters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/markdown.py` & `nbconvert-7.3.1/nbconvert/exporters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/notebook.py` & `nbconvert-7.3.1/nbconvert/exporters/notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/pdf.py` & `nbconvert-7.3.1/nbconvert/exporters/pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/python.py` & `nbconvert-7.3.1/nbconvert/exporters/python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/qt_exporter.py` & `nbconvert-7.3.1/nbconvert/exporters/qt_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/qt_screenshot.py` & `nbconvert-7.3.1/nbconvert/exporters/qt_screenshot.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/qtpdf.py` & `nbconvert-7.3.1/nbconvert/exporters/qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/rst.py` & `nbconvert-7.3.1/nbconvert/exporters/rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/script.py` & `nbconvert-7.3.1/nbconvert/exporters/script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/slides.py` & `nbconvert-7.3.1/nbconvert/exporters/slides.py`

 * *Files 2% similar despite different names*

```diff
@@ -120,15 +120,16 @@
     ).tag(config=True)
 
     @default("reveal_url_prefix")
     def _reveal_url_prefix_default(self):
         if "RevealHelpPreprocessor.url_prefix" in self.config:
             warn(
                 "Please update RevealHelpPreprocessor.url_prefix to "
-                "SlidesExporter.reveal_url_prefix in config files."
+                "SlidesExporter.reveal_url_prefix in config files.",
+                stacklevel=2,
             )
             return self.config.RevealHelpPreprocessor.url_prefix
         return "https://unpkg.com/reveal.js@4.0.2"
 
     reveal_theme = Unicode(
         "simple",
         help="""
```

### Comparing `nbconvert-7.3.0/nbconvert/exporters/templateexporter.py` & `nbconvert-7.3.1/nbconvert/exporters/templateexporter.py`

 * *Files 1% similar despite different names*

```diff
@@ -100,15 +100,15 @@
             target[k] = v
     return target  # return for convenience
 
 
 # define function at the top level to avoid pickle errors
 def deprecated(msg):
     """Emit a deprecation warning."""
-    warnings.warn(msg, DeprecationWarning)
+    warnings.warn(msg, DeprecationWarning, stacklevel=2)
 
 
 class ExtensionTolerantLoader(BaseLoader):
     """A template loader which optionally adds a given extension when searching.
 
     Constructor takes two arguments: *loader* is another Jinja loader instance
     to wrap. *extension* is the extension, which will be added to the template
@@ -206,14 +206,15 @@
     @validate("template_name")
     def _template_name_validate(self, change):
         template_name = change["value"]
         if template_name and template_name.endswith(".tpl"):
             warnings.warn(
                 f"5.x style template name passed '{self.template_name}'. Use --template-name for the template directory with a index.<ext>.j2 file and/or --template-file to denote a different template.",
                 DeprecationWarning,
+                stacklevel=2,
             )
             directory, self.template_file = os.path.split(self.template_name)
             if directory:
                 directory, template_name = os.path.split(directory)
             if directory and os.path.isabs(directory):
                 self.extra_template_basedirs = [directory]
         return template_name
@@ -231,14 +232,15 @@
             directory, self.template_file = os.path.split(full_path)
             self.extra_template_paths = [directory, *self.extra_template_paths]
             # While not strictly an invalid template file name, the extension hints that there isn't a template directory involved
             if self.template_file.endswith(".tpl"):
                 warnings.warn(
                     f"5.x style template file passed '{new}'. Use --template-name for the template directory with a index.<ext>.j2 file and/or --template-file to denote a different template.",
                     DeprecationWarning,
+                    stacklevel=2,
                 )
 
     @default("template_file")
     def _template_file_default(self):
         if self.template_extension:
             return "index" + self.template_extension
 
@@ -593,15 +595,15 @@
         """Get the base template config."""
         # Hard-coded base template confs to use for backwards compatibility for 5.x-only templates
         if name == "display_priority":
             return {"base_template": "base"}
         if name == "full":
             return {"base_template": "classic", "mimetypes": {"text/html": True}}
 
-    def get_template_names(self):
+    def get_template_names(self):  # noqa
         """Finds a list of template names where each successive template name is the base template"""
         template_names = []
         root_dirs = self.get_prefix_root_dirs()
         base_template = self.template_name
         merged_conf: dict = {}  # the configuration once all conf files are merged
         while base_template is not None:
             template_names.append(base_template)
@@ -631,14 +633,15 @@
                         root_dir, "nbconvert", "templates", "compatibility", compatibility_file
                     )
                     if os.path.exists(compatibility_path):
                         found_at_least_one = True
                         warnings.warn(
                             f"5.x template name passed '{self.template_name}'. Use 'lab' or 'classic' for new template usage.",
                             DeprecationWarning,
+                            stacklevel=2,
                         )
                         self.template_file = compatibility_file
                         conf = self.get_compatibility_base_template_conf(base_template)
                         self.template_name = conf.get("base_template")
                         break
                 if not found_at_least_one:
                     paths = "\n\t".join(root_dirs)
```

### Comparing `nbconvert-7.3.0/nbconvert/exporters/webpdf.py` & `nbconvert-7.3.1/nbconvert/exporters/webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/base.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/cheese.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/cheese.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_asciidoc.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_asciidoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_export.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_export.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_exporter.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_exporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_html.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_html.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_latex.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_markdown.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_notebook.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_notebook.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_pdf.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_python.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_python.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_qtpdf.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_qtpng.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_qtpng.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_rst.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_rst.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_script.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_script.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_slides.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_slides.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_templateexporter.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_templateexporter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/test_webpdf.py` & `nbconvert-7.3.1/nbconvert/exporters/tests/test_webpdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/attachment.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/attachment.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/notebook2.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/notebook3.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook3.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/notebook_inject.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/notebook_inject.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/pngmetadata.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/pngmetadata.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/prompt_numbers.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/prompt_numbers.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/rawtest.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/rawtest.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/exporters/tests/files/svg.ipynb` & `nbconvert-7.3.1/nbconvert/exporters/tests/files/svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/ansi.py` & `nbconvert-7.3.1/nbconvert/filters/ansi.py`

 * *Files 4% similar despite different names*

```diff
@@ -67,15 +67,15 @@
     text : unicode
         Text containing ANSI colors to convert to LaTeX
 
     """
     return _ansi2anything(text, _latexconverter)
 
 
-def _htmlconverter(fg, bg, bold, underline, inverse):
+def _htmlconverter(fg, bg, bold, underline, inverse):  # noqa
     """
     Return start and end tags for given foreground/background/bold/underline.
 
     """
     if (fg, bg, bold, underline, inverse) == (None, None, False, False, False):
         return "", ""
 
@@ -110,15 +110,15 @@
         starttag += ' class="' + " ".join(classes) + '"'
     if styles:
         starttag += ' style="' + "; ".join(styles) + '"'
     starttag += ">"
     return starttag, "</span>"
 
 
-def _latexconverter(fg, bg, bold, underline, inverse):
+def _latexconverter(fg, bg, bold, underline, inverse):  # noqa
     """
     Return start and end markup given foreground/background/bold/underline.
 
     """
     if (fg, bg, bold, underline, inverse) == (None, None, False, False, False):
         return "", ""
 
@@ -129,29 +129,29 @@
 
     if isinstance(fg, int):
         starttag += r"\textcolor{" + _ANSI_COLORS[fg] + "}{"
         endtag = "}" + endtag
     elif fg:
         # See http://tex.stackexchange.com/a/291102/13684
         starttag += r"\def\tcRGB{\textcolor[RGB]}\expandafter"
-        starttag += r"\tcRGB\expandafter{\detokenize{%s,%s,%s}}{" % fg
+        starttag += r"\tcRGB\expandafter{{\detokenize{{{},{},{}}}}}{{".format(*fg)
         endtag = "}" + endtag
     elif inverse:
         starttag += r"\textcolor{ansi-default-inverse-fg}{"
         endtag = "}" + endtag
 
     if isinstance(bg, int):
         starttag += r"\setlength{\fboxsep}{0pt}"
         starttag += r"\colorbox{" + _ANSI_COLORS[bg] + "}{"
         endtag = r"\strut}" + endtag
     elif bg:
         starttag += r"\setlength{\fboxsep}{0pt}"
         # See http://tex.stackexchange.com/a/291102/13684
         starttag += r"\def\cbRGB{\colorbox[RGB]}\expandafter"
-        starttag += r"\cbRGB\expandafter{\detokenize{%s,%s,%s}}{" % bg
+        starttag += r"\cbRGB\expandafter{{\detokenize{{{},{},{}}}}}{{".format(*bg)
         endtag = r"\strut}" + endtag
     elif inverse:
         starttag += r"\setlength{\fboxsep}{0pt}"
         starttag += r"\colorbox{ansi-default-inverse-bg}{"
         endtag = r"\strut}" + endtag
 
     if bold:
```

### Comparing `nbconvert-7.3.0/nbconvert/filters/citation.py` & `nbconvert-7.3.1/nbconvert/filters/citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/datatypefilter.py` & `nbconvert-7.3.1/nbconvert/filters/datatypefilter.py`

 * *Files 3% similar despite different names*

```diff
@@ -36,11 +36,12 @@
 
         """
         for fmt in self.display_data_priority:
             if fmt in output:
                 return [fmt]
         warn(
             "Your element with mimetype(s) {mimetypes}"
-            " is not able to be represented.".format(mimetypes=output.keys())
+            " is not able to be represented.".format(mimetypes=output.keys()),
+            stacklevel=2,
         )
 
         return []
```

### Comparing `nbconvert-7.3.0/nbconvert/filters/filter_links.py` & `nbconvert-7.3.1/nbconvert/filters/filter_links.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/highlight.py` & `nbconvert-7.3.1/nbconvert/filters/highlight.py`

 * *Files 4% similar despite different names*

```diff
@@ -42,15 +42,16 @@
         self.pygments_lexer = pygments_lexer or "ipython3"
         super().__init__(**kwargs)
 
     @observe("default_language")
     def _default_language_changed(self, change):
         warn(
             "Setting default_language in config is deprecated as of 5.0, "
-            "please use language_info metadata instead."
+            "please use language_info metadata instead.",
+            stacklevel=2,
         )
         self.pygments_lexer = change["new"]
 
     def __call__(self, source, language=None, metadata=None):
         """
         Return a syntax-highlighted version of the input source as html output.
 
@@ -98,15 +99,16 @@
         self.pygments_lexer = pygments_lexer or "ipython3"
         super().__init__(**kwargs)
 
     @observe("default_language")
     def _default_language_changed(self, change):
         warn(
             "Setting default_language in config is deprecated as of 5.0, "
-            "please use language_info metadata instead."
+            "please use language_info metadata instead.",
+            stacklevel=2,
         )
         self.pygments_lexer = change["new"]
 
     def __call__(self, source, language=None, metadata=None, strip_verbatim=False):
         """
         Return a syntax-highlighted version of the input source as latex output.
 
@@ -160,30 +162,30 @@
         language = metadata["magics_language"]
 
     lexer = None
     if language == "ipython2":
         try:
             from IPython.lib.lexers import IPythonLexer
         except ImportError:
-            warn("IPython lexer unavailable, falling back on Python")
+            warn("IPython lexer unavailable, falling back on Python", stacklevel=2)
             language = "python"
         else:
             lexer = IPythonLexer()
     elif language == "ipython3":
         try:
             from IPython.lib.lexers import IPython3Lexer
         except ImportError:
-            warn("IPython3 lexer unavailable, falling back on Python 3")
+            warn("IPython3 lexer unavailable, falling back on Python 3", stacklevel=2)
             language = "python3"
         else:
             lexer = IPython3Lexer()
 
     if lexer is None:
         try:
             lexer = get_lexer_by_name(language, stripall=True)
         except ClassNotFound:
-            warn("No lexer found for language %r. Treating as plain text." % language)
+            warn("No lexer found for language %r. Treating as plain text." % language, stacklevel=2)
             from pygments.lexers.special import TextLexer
 
             lexer = TextLexer()
 
     return highlight(source, lexer, output_formatter)
```

### Comparing `nbconvert-7.3.0/nbconvert/filters/latex.py` & `nbconvert-7.3.1/nbconvert/filters/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/markdown.py` & `nbconvert-7.3.1/nbconvert/filters/markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/markdown_mistune.py` & `nbconvert-7.3.1/nbconvert/filters/markdown_mistune.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/pandoc.py` & `nbconvert-7.3.1/nbconvert/filters/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/strings.py` & `nbconvert-7.3.1/nbconvert/filters/strings.py`

 * *Files 1% similar despite different names*

```diff
@@ -230,15 +230,16 @@
         IPython code, to be transformed to pure Python
     """
     try:
         from IPython.core.inputtransformer2 import TransformerManager
     except ImportError:
         warnings.warn(
             "IPython is needed to transform IPython syntax to pure Python."
-            " Install ipython if you need this functionality."
+            " Install ipython if you need this functionality.",
+            stacklevel=2,
         )
         return code
     else:
         isp = TransformerManager()
         return isp.transform_cell(code)
```

### Comparing `nbconvert-7.3.0/nbconvert/filters/svg_constants.py` & `nbconvert-7.3.1/nbconvert/filters/svg_constants.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/widgetsdatatypefilter.py` & `nbconvert-7.3.1/nbconvert/filters/widgetsdatatypefilter.py`

 * *Files 5% similar despite different names*

```diff
@@ -67,11 +67,12 @@
                     and output[WIDGET_VIEW_MIMETYPE]["model_id"] not in widgets_state
                 ):
                     continue
 
                 return [fmt]
         warn(
             "Your element with mimetype(s) {mimetypes}"
-            " is not able to be represented.".format(mimetypes=output.keys())
+            " is not able to be represented.".format(mimetypes=output.keys()),
+            stacklevel=2,
         )
 
         return []
```

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_ansi.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_ansi.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_citation.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_citation.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_datatypefilter.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_datatypefilter.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_highlight.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_highlight.py`

 * *Files 1% similar despite different names*

```diff
@@ -66,15 +66,15 @@
             self._try_highlight(highlight2latex, test, self.tokens[index])
 
     def test_parse_html_many_lang(self):
         ht = highlight2html(self.tests[0])
         rb = highlight2html_ruby(self.tests[0])
 
         for lang, tkns in [(ht, ("def",)), (rb, ("def", "end"))]:
-            root = xml.etree.ElementTree.fromstring(lang)
+            root = xml.etree.ElementTree.fromstring(lang)  # noqa
             self.assertEqual(self._extract_tokens(root, "k"), set(tkns))
 
     @pytest.mark.filterwarnings("ignore")
     def test_inject_html(self):
         out = highlight2html(self.tests[0], 'ipython3-foo"><script>alert(1)</script>')
         assert "<script>alert(1)</script>" not in out
```

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_latex.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_markdown.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_markdown.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_metadata.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_metadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/filters/tests/test_strings.py` & `nbconvert-7.3.1/nbconvert/filters/tests/test_strings.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/postprocessors/base.py` & `nbconvert-7.3.1/nbconvert/postprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/postprocessors/serve.py` & `nbconvert-7.3.1/nbconvert/postprocessors/serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/postprocessors/tests/test_serve.py` & `nbconvert-7.3.1/nbconvert/postprocessors/tests/test_serve.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/__init__.py` & `nbconvert-7.3.1/nbconvert/preprocessors/__init__.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/base.py` & `nbconvert-7.3.1/nbconvert/preprocessors/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/clearmetadata.py` & `nbconvert-7.3.1/nbconvert/preprocessors/clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/clearoutput.py` & `nbconvert-7.3.1/nbconvert/preprocessors/clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/coalescestreams.py` & `nbconvert-7.3.1/nbconvert/preprocessors/coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/convertfigures.py` & `nbconvert-7.3.1/nbconvert/preprocessors/convertfigures.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/csshtmlheader.py` & `nbconvert-7.3.1/nbconvert/preprocessors/csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/execute.py` & `nbconvert-7.3.1/nbconvert/preprocessors/execute.py`

 * *Files 2% similar despite different names*

```diff
@@ -20,14 +20,15 @@
     """DEPRECATED."""
     from warnings import warn
 
     warn(
         "The 'nbconvert.preprocessors.execute.executenb' function was moved to nbclient.execute. "
         "We recommend importing that library directly.",
         FutureWarning,
+        stacklevel=2,
     )
     return _execute(*args, **kwargs)
 
 
 # We inherit from both classes to allow for traitlets to resolve as they did pre-6.0.
 # This unfortunately makes for some ugliness around initialization as NotebookClient
 # assumes it's a constructed class with a nb object that we have to hack around.
@@ -37,15 +38,14 @@
     """
 
     def __init__(self, **kw):
         """Initialize the preprocessor."""
         nb = kw.get("nb")
         if nb is None:
             nb = NotebookNode()
-        kw.setdefault("kernel_manager_class", KernelManager)
         Preprocessor.__init__(self, nb=nb, **kw)
         NotebookClient.__init__(self, nb, **kw)
 
     def _check_assign_resources(self, resources):
         if resources or not hasattr(self, "resources"):
             self.resources = resources
```

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/extractoutput.py` & `nbconvert-7.3.1/nbconvert/preprocessors/extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/highlightmagics.py` & `nbconvert-7.3.1/nbconvert/preprocessors/highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/latex.py` & `nbconvert-7.3.1/nbconvert/preprocessors/latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/regexremove.py` & `nbconvert-7.3.1/nbconvert/preprocessors/regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/sanitize.py` & `nbconvert-7.3.1/nbconvert/preprocessors/sanitize.py`

 * *Files 3% similar despite different names*

```diff
@@ -26,21 +26,23 @@
         from bleach import ALLOWED_STYLES  # type:ignore
 
         _USE_BLEACH_CSS_SANITIZER = False
         _USE_BLEACH_STYLES = True
         warnings.warn(
             "Support for bleach <5 will be removed in a future version of nbconvert",
             DeprecationWarning,
+            stacklevel=2,
         )
 
     except ImportError:
         warnings.warn(
             "The installed bleach/tinycss2 do not provide CSS sanitization, "
             "please upgrade to bleach >=5",
             UserWarning,
+            stacklevel=2,
         )
 
 
 __all__ = ["SanitizeHTML"]
 
 
 class SanitizeHTML(Preprocessor):
```

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/svg2pdf.py` & `nbconvert-7.3.1/nbconvert/preprocessors/svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tagremove.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/base.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/fake_kernelmanager.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/fake_kernelmanager.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_clearmetadata.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearmetadata.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_clearoutput.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_clearoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_coalescestreams.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_coalescestreams.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_csshtmlheader.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_csshtmlheader.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_execute.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_execute.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_extractoutput.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_extractoutput.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_highlightmagics.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_highlightmagics.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_latex.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_latex.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_regexremove.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_regexremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_sanitize.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_sanitize.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_svg2pdf.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_svg2pdf.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/test_tagremove.py` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/test_tagremove.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb` & `nbconvert-7.3.1/nbconvert/preprocessors/tests/files/MixedMarkdown.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/templates/skeleton/Makefile` & `nbconvert-7.3.1/nbconvert/templates/skeleton/Makefile`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/base.py` & `nbconvert-7.3.1/nbconvert/tests/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/fake_exporters.py` & `nbconvert-7.3.1/nbconvert/tests/fake_exporters.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/test_nbconvertapp.py` & `nbconvert-7.3.1/nbconvert/tests/test_nbconvertapp.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/Unexecuted_widget.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/Unexecuted_widget_2.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/Unexecuted_widget_2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/Widget_List.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/Widget_List.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/containerized_deployments.jpeg` & `nbconvert-7.3.1/nbconvert/tests/files/containerized_deployments.jpeg`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/issue1849_svg.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/issue1849_svg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/latex-linked-image.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/latex-linked-image.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/markdown_display_priority.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/markdown_display_priority.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/notebook1.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/notebook1.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/notebook2.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/notebook2.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/notebook3_with_errors.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/notebook3_with_errors.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/notebook4_jpeg.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/notebook4_jpeg.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/notebook5_embed_images.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/notebook5_embed_images.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/notebook_tags.ipynb` & `nbconvert-7.3.1/nbconvert/tests/files/notebook_tags.ipynb`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/tests/files/testimage.png` & `nbconvert-7.3.1/nbconvert/tests/files/testimage.png`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/_contextlib_chdir.py` & `nbconvert-7.3.1/nbconvert/utils/_contextlib_chdir.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/base.py` & `nbconvert-7.3.1/nbconvert/utils/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/exceptions.py` & `nbconvert-7.3.1/nbconvert/utils/exceptions.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/io.py` & `nbconvert-7.3.1/nbconvert/utils/io.py`

 * *Files 0% similar despite different names*

```diff
@@ -99,15 +99,15 @@
     if link_errno == errno.EEXIST:
         if os.stat(src).st_ino == os.stat(dst).st_ino:
             # dst is already a hard link to the correct file, so we don't need
             # to do anything else. If we try to link and rename the file
             # anyway, we get duplicate files - see http://bugs.python.org/issue21876
             return
 
-        new_dst = dst + f"-temp-{random.randint(1, 16**4):04X}"
+        new_dst = dst + f"-temp-{random.randint(1, 16**4):04X}"  # noqa
         try:
             link_or_copy(src, new_dst)
         except BaseException:
             try:
                 os.remove(new_dst)
             except OSError:
                 pass
```

### Comparing `nbconvert-7.3.0/nbconvert/utils/pandoc.py` & `nbconvert-7.3.1/nbconvert/utils/pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/text.py` & `nbconvert-7.3.1/nbconvert/utils/text.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/version.py` & `nbconvert-7.3.1/nbconvert/utils/version.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/tests/test_io.py` & `nbconvert-7.3.1/nbconvert/utils/tests/test_io.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/utils/tests/test_pandoc.py` & `nbconvert-7.3.1/nbconvert/utils/tests/test_pandoc.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/writers/base.py` & `nbconvert-7.3.1/nbconvert/writers/base.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/writers/debug.py` & `nbconvert-7.3.1/nbconvert/writers/debug.py`

 * *Files 1% similar despite different names*

```diff
@@ -35,11 +35,11 @@
 
         See base for more...
         """
 
         if isinstance(resources["outputs"], dict):
             print("outputs extracted from %s" % notebook_name)
             print("-" * 80)
-            pprint(resources["outputs"], indent=2, width=70)
+            pprint(resources["outputs"], indent=2, width=70)  # noqa
         else:
             print("no outputs extracted from %s" % notebook_name)
         print("=" * 80)
```

### Comparing `nbconvert-7.3.0/nbconvert/writers/files.py` & `nbconvert-7.3.1/nbconvert/writers/files.py`

 * *Files 1% similar despite different names*

```diff
@@ -96,15 +96,15 @@
 
         # Copy referenced files to output directory
         if build_directory:
             for filename in self.files:
                 # Copy files that match search pattern
                 for matching_filename in glob.glob(filename):
                     # compute the relative path for the filename
-                    if relpath != "":
+                    if relpath != "":  # noqa
                         dest_filename = os.path.relpath(matching_filename, relpath)
                     else:
                         dest_filename = matching_filename
 
                     # Make sure folder exists.
                     dest = os.path.join(build_directory, dest_filename)
                     path = os.path.dirname(dest)
```

### Comparing `nbconvert-7.3.0/nbconvert/writers/stdout.py` & `nbconvert-7.3.1/nbconvert/writers/stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/writers/tests/test_debug.py` & `nbconvert-7.3.1/nbconvert/writers/tests/test_debug.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/writers/tests/test_files.py` & `nbconvert-7.3.1/nbconvert/writers/tests/test_files.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/nbconvert/writers/tests/test_stdout.py` & `nbconvert-7.3.1/nbconvert/writers/tests/test_stdout.py`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/asciidoc/index.asciidoc.j2` & `nbconvert-7.3.1/share/templates/asciidoc/index.asciidoc.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/base/display_priority.j2` & `nbconvert-7.3.1/share/templates/base/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/base/jupyter_widgets.html.j2` & `nbconvert-7.3.1/share/templates/base/jupyter_widgets.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/base/mathjax.html.j2` & `nbconvert-7.3.1/share/templates/base/mathjax.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/base/null.j2` & `nbconvert-7.3.1/share/templates/base/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/classic/base.html.j2` & `nbconvert-7.3.1/share/templates/classic/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/classic/index.html.j2` & `nbconvert-7.3.1/share/templates/classic/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/classic/static/style.css` & `nbconvert-7.3.1/share/templates/classic/static/style.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/lab/base.html.j2` & `nbconvert-7.3.1/share/templates/lab/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/lab/index.html.j2` & `nbconvert-7.3.1/share/templates/lab/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/lab/static/index.css` & `nbconvert-7.3.1/share/templates/lab/static/index.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/lab/static/theme-dark.css` & `nbconvert-7.3.1/share/templates/lab/static/theme-dark.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/lab/static/theme-light.css` & `nbconvert-7.3.1/share/templates/lab/static/theme-light.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/base.tex.j2` & `nbconvert-7.3.1/share/templates/latex/base.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/display_priority.j2` & `nbconvert-7.3.1/share/templates/latex/display_priority.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/document_contents.tex.j2` & `nbconvert-7.3.1/share/templates/latex/document_contents.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/null.j2` & `nbconvert-7.3.1/share/templates/latex/null.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/report.tex.j2` & `nbconvert-7.3.1/share/templates/latex/report.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/style_bw_ipython.tex.j2` & `nbconvert-7.3.1/share/templates/latex/style_bw_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/style_ipython.tex.j2` & `nbconvert-7.3.1/share/templates/latex/style_ipython.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/style_jupyter.tex.j2` & `nbconvert-7.3.1/share/templates/latex/style_jupyter.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/latex/style_python.tex.j2` & `nbconvert-7.3.1/share/templates/latex/style_python.tex.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/markdown/index.md.j2` & `nbconvert-7.3.1/share/templates/markdown/index.md.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/reveal/base.html.j2` & `nbconvert-7.3.1/share/templates/reveal/base.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/reveal/index.html.j2` & `nbconvert-7.3.1/share/templates/reveal/index.html.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/reveal/static/custom_reveal.css` & `nbconvert-7.3.1/share/templates/reveal/static/custom_reveal.css`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/share/templates/rst/index.rst.j2` & `nbconvert-7.3.1/share/templates/rst/index.rst.j2`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/.gitignore` & `nbconvert-7.3.1/.gitignore`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/LICENSE` & `nbconvert-7.3.1/LICENSE`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/README.md` & `nbconvert-7.3.1/README.md`

 * *Files identical despite different names*

### Comparing `nbconvert-7.3.0/hatch_build.py` & `nbconvert-7.3.1/hatch_build.py`

 * *Files 0% similar despite different names*

```diff
@@ -43,15 +43,15 @@
     """Get a css file and download it to the templates dir"""
     directory = osp.join(templates_dir, template_name, "static")
     dest = osp.join(directory, filename)
     if not osp.exists(directory):
         os.makedirs(directory)
     print("Downloading CSS: %s" % url)
     try:
-        css = urlopen(url).read()
+        css = urlopen(url).read()  # noqa
     except Exception as e:
         msg = f"Failed to download css from {url}: {e}"
         print(msg, file=sys.stderr)
         if osp.exists(dest):
             print("Already have CSS: %s, moving on." % dest)
         else:
             msg = "Need CSS to proceed."
```

### Comparing `nbconvert-7.3.0/pyproject.toml` & `nbconvert-7.3.1/pyproject.toml`

 * *Files 1% similar despite different names*

```diff
@@ -122,18 +122,18 @@
 features = ["test"]
 dependencies = ["mypy>=0.990"]
 [tool.hatch.envs.typing.scripts]
 test = "mypy --install-types --non-interactive {args:nbconvert}"
 
 [tool.hatch.envs.lint]
 dependencies = [
-  "black[jupyter]==23.1.0",
+  "black[jupyter]==23.3.0",
   "mdformat>0.7",
   "mdformat-gfm>=0.3.5",
-  "ruff==0.0.254"
+  "ruff==0.0.260"
 ]
 detached = true
 [tool.hatch.envs.lint.scripts]
 style = [
   "ruff {args:.}",
   "black --check --diff {args:.}",
   "mdformat --check {args:docs *.md}"
```

### Comparing `nbconvert-7.3.0/PKG-INFO` & `nbconvert-7.3.1/PKG-INFO`

 * *Files 2% similar despite different names*

```diff
@@ -1,10 +1,10 @@
 Metadata-Version: 2.1
 Name: nbconvert
-Version: 7.3.0
+Version: 7.3.1
 Summary: Converting Jupyter Notebooks
 Project-URL: Homepage, https://jupyter.org
 Author-email: Jupyter Development Team <jupyter@googlegroups.com>
 License: BSD 3-Clause License
         
         - Copyright (c) 2001-2015, IPython Development Team
         - Copyright (c) 2015-, Jupyter Development Team
```

