---
title: "On the Complexity of Network-Wide Configuration Synthesis"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Roland Schmid
- Laurent Vanbever

# Author notes (optional)
author_notes:
- ""
- ""
- ""

date: "2022-11-23T00:00:00Z"
doi: "10.1109/ICNP55882.2022.9940325"

# Schedule page publish date (NOT publication's date).
publishDate: "2022-11-23T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *2022 IEEE 30th International Conference on Network Protocols*
publication_short: In *ICNP'22*

abstract: Configuration Synthesis promises to increase automation in network hardware configuration but is generally assumed to constitute a computationally hard problem. We conduct a formal analysis of the computational complexity of network-wide Configuration Synthesis to establish this claim formally. To that end, we consider Configuration Synthesis as a decision problem, whether or not the selected routing protocol(s) can implement a given set of forwarding properties.<br /><br />We find the complexity of Configuration Synthesis heavily depends on the combination of the forwarding properties that need to be implemented in the network, as well as the employed routing protocol(s). Our analysis encompasses different forwarding properties that can be encoded as path constraints, and any combination of distributed destination-based hop-by-hop routing protocols. Many of these combinations yield NP-hard Configuration Synthesis problems; in particular, we show that the satisfiability of a set of arbitrary waypoints for any hop-by-hop routing protocol is NP-complete. Other combinations, however, show potential for efficient, scalable Configuration Synthesis.

# Summary. An optional shortened abstract.
summary: Large-scale reconfiguraiton campaigns in internet networks typically introduce downtimes, decrease performance, and violate security policies. *Snowcap* solves this issue by safely and automatically reconfiguring the netowrk step-by-step.

tags: 
- Network management
- Configuration Synthesis
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
