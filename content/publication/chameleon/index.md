---
title: "Taming the transient while reconfiguring BGP"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Roland Schmid
- Stefano Vissicchio
- Laurent Vanbever

# Author notes (optional)
author_notes:
- ""
- ""
- ""

date: "2023-09-01T00:00:00Z"
doi: "10.1145/3603269.3604855"

# Schedule page publish date (NOT publication's date).
publishDate: "2023-09-01T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *ACM Special Interest Group on Data Communications 2023*
publication_short: In *SIGCOMM'23*

abstract: 'BGP reconfigurations are a daily occurrence for most network operators, especially in large networks. Yet, performing safe and robust BGP reconfiguration changes is still an open problem. Few BGP reconfiguration techniques exist, and they are either (i) unsafe, because they ignore transient states, which can easily lead to invariant violations; or (ii) impractical, as they duplicate the entire routing and forwarding states, and require special hardware. In this paper, we introduce Chameleon, the first BGP reconfiguration framework capable of maintaining correctness throughout a reconfiguration campaign while relying on standard BGP functionalities and minimizing state duplication. Akin to concurrency coordination in distributed systems, Chameleon models the reconfiguration process with happens-before relations. This modeling allows us to capture the safety properties of transient BGP states. We then use this knowledge to precisely control the BGP route propagation and convergence, so that input invariants are provably preserved at any time during the reconfiguration. We fully implement Chameleon and evaluate it in both testbeds and simulations, on real-world topologies and large-scale reconfiguration scenarios. In most experiments, our system computes reconfiguration plans within a minute, and performs them from start to finish in a few minutes, with minimal overhead.'

# Summary. An optional shortened abstract.
summary: 'Chameleon performs any BGP reconfiguration while providing strong forwarding guarantees in any state during the convergence, even transient ones.'

tags: 
- Network management
- Network reliability
- Logic and verification

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'chameleon.pdf'
url_code: 'https://github.com/nsg-ethz/chameleon'
url_dataset: ''
url_poster: ''
url_project: 'https://chameleon.ethz.ch'
url_slides: 'chameleon_slides.pdf'
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
- chameleon

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
