+++
title = "MC Mutants: Evaluating and Improving Testing for Memory Consistency Specifications"
date = 2023-09-01T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["R. Levine", "T. Guo", "M. Cho", "A. Baker", "R. Levien", "D. Neto", "A. Quinn", "T. Sorensen"]

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
publication_short = "In *ASPLOS*"

# Abstract and optional shortened version.

abstract = "Shared memory platforms (i.e., compute devices, drivers, and compilers) provide a memory consistency specification (MCS) so that developers can reason about the behaviors of their parallel programs.  Unfortunately, ensuring that a platform conforms to its MCS is difficult, as is exemplified by numerous bugs in well-used platforms.  While existing MCS testing approaches find bugs, their efficacy depends on the testing environment (e.g., if synthetic memory pressure is applied). MCS testing environments are difficult to evaluate since legitimate MCS violations are too rare to use as an efficacy metric. As a result, prior approaches have missed critical MCS bugs. <br> This work proposes a mutation testing approach for evaluating MCS testing environments: MC Mutants. This approach mutates MCS tests such that the mutants simulate bugs that might occur.  A testing environment can then be evaluated using a mutation score. We utilize MC Mutants in two novel contributions: (1) a parallel testing environment, and (2) An MCS testing confidence strategy that is parameterized over a time budget and confidence threshold.  We implement our contributions in WebGPU, a new web-based GPU programming specification, and evaluate our techniques across four GPUs. We improve testing speed by three orders of magnitude over prior work, empowering us to create a conformance test suite that reproduces many mutated tests with high confidence and requires only 64 seconds per test. We identified two bugs in WebGPU implementations, one of which led to a specification change. Moreover, the official WebGPU conformance test suite has adopted our approach due to its efficiency, effectiveness, and broad applicability."

abstract_short = ""

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
url_pdf = "https://reeselevine.github.io/assets/pdf/mc_mutants.pdf"
links = [{name="News",url="https://news.ucsc.edu/2023/03/sorensen-bugs.html"}]
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = ""
url_slides = ""
url_video = ""
url_poster = ""
url_source = ""

# Custom links (optional).
#   Uncomment line below to enable. For multiple links, use the form `[{...}, {...}, {...}]`.
# url_custom = [{name = "Custom Link", url = "http://example.org"}]

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