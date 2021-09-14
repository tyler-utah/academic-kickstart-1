+++
title = "Specifying and Testing GPU Workgroup Progress Models"
date = 2021-09-03T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["T. Sorensen", "L. F. Salvador", "H. Raval", "H. Evrard", "J. Wickerson", "M. Martonosi", "A. F. Donaldson"]

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
abstract = "As GPU availability has increased and programming support has matured, a wider variety of applications are being ported to these platforms. Many parallel applications contain fine-grained synchronization idioms; as such, their correct execution depends on a degree of relative forward progress between threads (or thread groups). Unfortunately, many GPU programming specifications (e.g. Vulkan and Metal) say almost nothing about relative forward progress guarantees between workgroups. Although prior work has proposed a spectrum of plausible progress models for GPUs, cross-vendor specifications have yet to commit to any model. This work is a collection of tools and experimental data to aid specification designers when considering forward progress guarantees in programming frameworks. As a foundation, we formalize a small parallel programming language that captures the essence of fine-grained synchronization. We then provide a means of formally specifying a progress model, and develop a termination oracle that decides whether a given program is guaranteed to eventually terminate with respect to a given progress model. Next, we formalize a set of constraints that describe concurrent programs that require forward progress to terminate. This allows us to synthesize a large set of 483 progress litmus tests. Combined with the termination oracle, we can determine the expected status of each litmus test -- i.e. whether it is guaranteed to eventually terminate -- under various progress models.  We present a large experimental campaign running the litmus tests across 8 GPUs from 5 different vendors. Our results highlight that GPUs have significantly different termination behaviors under our test suite. Most notably, we find that Apple and ARM GPUs do not support the linear occupancy-bound model, as was hypothesized by prior work."


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
url_pdf = "files/oopsla2021b.pdf"
url_preprint = ""
url_code = "https://github.com/tyler-utah/AlloyForwardProgress/tree/master/artifact"
links = [{name="Test Explorer",url="https://www.cs.princeton.edu/~ls24/testExplorer.html?threads=2&instructions=2&test=0"}]
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
