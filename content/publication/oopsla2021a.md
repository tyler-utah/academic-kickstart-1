+++
title = "The Semantics of Shared Memory in Intel CPU/FPGASystems"
date = 2021-09-02T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["D. Iorga", "A. F. Donaldson", "T. Sorensen", "J. Wickerson"]

# Publication type.
# Legend:
# 0 = Uncategorized
# 1 = Conference paper
# 2 = Journal article
# 3 = Manuscript
# 4 = Report
# 5 = Book
# 6 = Book section
publication_types = ["1"]

# Publication name and optional abbreviated version.
publication_short = "In _OOPSLA_"

# Abstract and optional shortened version.
abstract = "Heterogeneous CPU/FPGA devices, in which a CPU and an FPGA can execute together while sharing memory, are becoming popular in several computing sectors. In this paper, we study the shared-memory semantics of these devices, with a view to providing a firm foundation for reasoning about the programs that run on them. Our focus is on Intel platforms that combine an Intel FPGA with a multicore Xeon CPU. We describe the weak-memory behaviours that are allowed (and observable) on these devices when CPU threads and an FPGA thread access common memory locations in a fine-grained manner through multiple channels. Some of these behaviours are familiar from well-studied CPU and GPU concurrency; others are weaker still. We encode these behaviours in two formal memory models: one operational, one axiomatic. We develop executable implementations of both models, using the CBMC bounded model-checking tool for our operational model and the Alloy modelling language for our axiomatic model. Using these, we cross-check our models against each other via a translator that converts Alloy-generated executions into queries for the CBMC model. We also validate our models against actual hardware by translating 583 Alloy-generated executions into litmus tests that we run on CPU/FPGA devices; when doing this, we avoid the prohibitive cost of synthesising a hardware design per litmus test by creating our own `litmus-test processor' in hardware. We expect that our models will be useful for low-level programmers, compiler writers, and designers of analysis tools. Indeed, as a demonstration of the utility of our work, we use our operational model to reason about a producer/consumer buffer implemented across the CPU and the FPGA. When the buffer uses insufficient synchronisation -- a situation that our model is able to detect -- we observe that its performance improves at the cost of occasional data corruption."


# Featured image thumbnail (optional)
image_preview = ""

# Is this a selected publication? (true/false)
selected = false

# Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's filename without extension.
#   E.g. `projects = ["deep-learning"]` references `content/project/deep-learning.md`.
#   Otherwise, set `projects = []`.
projects = []

# Tags (optional).
#   Set `tags = []` for no tags, or use the form `tags = ["A Tag", "Another Tag"]` for one or more tags.
tags = []

# Links (optional).
url_pdf = "files/oopsla2021a.pdf"
url_preprint = ""
url_code = "https://github.com/diorga/harpy"
#url_custom = [{name = "blog post", url="https://johnwickerson.wordpress.com/2021/07/03/understanding-the-memory-semantics-of-multi-threaded-cpu-fpga-programs/"}]
links = [{name="Blog",url="https://johnwickerson.wordpress.com/2021/07/03/understanding-the-memory-semantics-of-multi-threaded-cpu-fpga-programs/"}]
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
url_custom = [{name = "Custom Link", url = "http://example.org"}]

# Does this page contain LaTeX math? (true/false)
math = true

# Does this page require source code highlighting? (true/false)
highlight = true

# Featured image
# Place your image in the `static/img/` folder and reference its filename below, e.g. `image = "example.jpg"`.
[header]
image = ""
caption = ""
+++
