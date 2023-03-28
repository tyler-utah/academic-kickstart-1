+++
title = "Redwood: Flexible and Portable Heterogeneous Tree Traversal Workloads"
date = 2023-02-01T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["Y. Xu", "A. Li", "T. Sorensen"]

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
publication_short = "in *ISPASS*"

# Abstract and optional shortened version.

abstract = "Shared memory heterogeneous systems are now mainstream, with nearly every mobile phone and tablet containing integrated processing units.  However, developing applications for such devices is difficult as workloads must be decomposed across different processing units, and the decomposition must be flexible to account for the growing diversity of devices, each with different relative processing unit throughput.  Furthermore, many devices require distinct programming front ends, requiring significant effort to write cross-platform applications. <br> In this work, we identify a pragmatic class of applications, which we call traverse-compute applications, that are ideal for shared memory heterogeneous systems. These applications have a flexible heterogeneous decomposition where CPUs excel at traversing a tree structure, while accelerators excel at node computations.  Leveraging this insight, we present Redwood: a framework for writing heterogeneous traverse-compute workloads. Redwood provides a simple processing unit abstraction and a tree traversal library that enables heterogeneous optimizations.  Using Redwood, we implement Grove, a benchmark suite containing nine pragmatic tree traversal applications, e.g., k-nearest neighbors.  We instantiate Redwood for three different heterogeneous programming platforms: CUDA, SYCL, and High-Level Synthesis; we use Grove to evaluate five shared memory heterogeneous systems.  Our evaluation highlights the importance of flexible heterogeneous decomposition as the optimal parameters differ widely across platforms and applications.  However, once optimally configured, heterogeneous implementations can provide up to $13.53x$ speedups (geomean of $3.01x$) over homogeneous implementations, showcasing the potential of heterogeneous computing for these workloads."

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
url_pdf = "files/ispass2023.pdf"
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
