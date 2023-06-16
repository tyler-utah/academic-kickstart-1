+++
title = "GPUHarbor: Testing GPU Memory Consistency at Large (Experience Paper)"
date = 2023-06-01T00:00:00
draft = false

# Authors. Comma separated list, e.g. `["Bob Smith", "David Jones"]`.
# authors = ["R. Levine", "T. Guo", "M. Cho", "A. Baker", "R. Levien", "D. Neto", "A. Quinn", "T. Sorensen"]
authors = ["R. Levine", "M. Cho", "D. McKee", "A. Quinn", "T. Sorensen"]

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
publication_short = "in *ISSTA*"

# Abstract and optional shortened version.

abstract = "Memory consistency specifications (MCSs) are a difficult, yet critical, part of a concurrent programming framework. Existing MCS testing tools are not immediately accessible, and thus, they have only been applied to a limited number of platforms. However, in the post-Dennard scaling landscape, there has been an explosion of new architectures and frameworks, especially for GPUs. Studying the shared memory behaviors of different devices (across vendors and architecture generations) is important to ensure conformance and to understand the extent that devices show different behaviors.  In this paper, we present GPUHarbor, a widescale GPU MCS testing tool. GPUHarbor has two interfaces: a web interface and an Android app. Using GPUHarbor, we deployed a testing campaign that checks conformance and characterizes weak behaviors. We advertised GPUHarbor on forums and social media, allowing us to collect testing data from 106 devices, spanning seven vendors.  In terms of devices tested, this constitutes the largest study on weak memory behaviors by at least 10×, and our conformance tests identified two new bugs on embedded Arm and NVIDIA devices. Analyzing our characterization data yields many insights, including quantifying and comparing weak behavior occurrence rates (e.g., AMD GPUs show 25.3× more weak behaviors on average than Intel). We conclude with a discussion of the impact our results have on software development for these performance-critical devices."

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
url_pdf = "https://reeselevine.github.io/assets/pdf/gpuharbor.pdf"
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
