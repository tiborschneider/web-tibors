---
title: "Snowcap: Synthesizing Network-Wide Configuration Updates"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Rüdiger Birkner
- Laurent Vanbever

# Author notes (optional)
author_notes:
- ""
- ""
- ""

date: "2021-08-23T00:00:00Z"
doi: "10.1145/3452296.3472915"

# Schedule page publish date (NOT publication's date).
publishDate: "2021-07-03T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *ACM Special Interest Group on Data Communications 2021*
publication_short: In *SIGCOMM'21*

abstract: Large-scale reconfiguration campaigns tend to be nerve-racking for network operators as they can lead to significant network downtimes, decreased performance, and policy violations. Unfortunately, existing reconfiguration frameworks often fall short in practice as they either only support a small set of reconfiguration scenarios or simply do not scale.<br /><br />We address these problems with Snowcap, the first network reconfiguration framework which can synthesize configuration updates that comply with arbitrary hard and soft specifications, and involve arbitrary routing protocols. Our key contribution is an efficient search procedure which leverages counter-examples to efficiently navigate the space of configuration updates. Given a reconfiguration ordering which violates the desired specifications, our algorithm automatically identifies the problematic commands so that it can avoid this particular order in the next iteration.<br /><br />We fully implemented Snowcap and extensively evaluated its scalability and effectiveness on real-world topologies and typical, large-scale reconfiguration scenarios. Even for large topologies, Snowcap finds a valid reconfiguration ordering with minimal side-effects (i.e., traffic shifts) within a few seconds at most.

# Summary. An optional shortened abstract.
summary: Large-scale reconfiguraiton campaigns in internet networks typically introduce downtimes, decrease performance, and violate security policies. *Snowcap* solves this issue by safely and automatically reconfiguring the netowrk step-by-step.

tags: 
- Network management
- Network reliability
- Network simulations
- Modal and temporal logics
- Logic and verification

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'snowcap.pdf'
url_code: 'https://github.com/nsg-ethz/snowcap'
url_dataset: ''
url_poster: ''
url_project: 'https://snowcap.ethz.ch/public/index.html'
url_slides: 'snowcap_slides.pdf'
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder. 
image:
  caption: 'Icon'
  focal_point: ""
  preview_only: true

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
- snowcap

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
