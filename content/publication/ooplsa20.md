+++
title = "Foundations of Empirical Memory Consistency Testing"
date = 2020-10-01T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
authors = ["J. Kirkham", "T. Sorensen", "E. Tureci", "M. Martonosi"]

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
publication_short = "In *OOPSLA*"

# Abstract and optional shortened version.
abstract = "Modern memory consistency models are complex, and it is difficult to reason about the relaxed behaviors that current systems allow. Programming languages, such as C and OpenCL, offer a memory model interface that developers can use to safely write concurrent applications. This abstraction provides functional portability across any platform that implements the interface, regardless of differences in the underlying systems. This powerful abstraction hinges on the ability of the system to correctly implement the interface. Many techniques for memory consistency model validation use empirical testing, which has been effective at uncovering undocumented behaviors and even finding bugs in trusted compilation schemes. Memory model testing consists of small concurrent unit tests called litmus tests. In these tests, certain observations, including potential bugs, are exceedingly rare, as they may only be triggered by precise interleaving of system steps in a complex processor, which is probabilistic in nature. Thus, each test must be run many times in order to provide a high level of confidence in its coverage. In this work, we rigorously investigate empirical memory model testing. In particular, we propose methodologies for navigating complex stressing routines and analyzing large numbers of testing observations. Using these insights, we can more efficiently tune stressing parameters, which can lead to higher confidence results at a faster rate. We emphasize the need for such approaches by performing a meta-study of prior work, which reveals results with low reproducibility and inefficient use of testing time. Our investigation is presented alongside empirical data. We believe that OpenCL targeting GPUs is a pragmatic choice in this domain as there exists a variety of different platforms to test, from large HPC servers to power-efficient edge devices. The tests presented in the work span 3 GPUs from 3 different vendors. We show that our methodologies are applicable across the GPUs, despite significant variances in the results. Concretely, our results show: lossless speedups of more than 5 in tuning using data peeking; a definition of portable stressing parameters which loses only 12% efficiency when generalized across our domain; a priority order of litmus tests for tuning. We stress test a conformance test suite for the OpenCL 2.0 memory model and discover a bug in Intel's compiler. Our methods are evaluated on the other two GPUs using mutation testing. We end with recommendations for official memory model conformance tests."


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
url_pdf = "files/oopsla2020.pdf"           
url_preprint = ""
url_code = ""
url_dataset = ""
url_project = ""
url_slides = ""
url_video = "https://www.youtube.com/watch?v=-Vxip6eQzgo"
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
