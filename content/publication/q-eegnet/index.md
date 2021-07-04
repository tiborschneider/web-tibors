---
title: "Q-EEGNET: an Energy-Efficient 8-bit Quantized Parallel EEGNet Implementation for Edge Motor-Imagery Brain-Machine Interfaces"

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here 
# and it will be replaced with their full name and linked to their profile.
authors:
- admin
- Xiaying Wang
- Michael Hersche
- Lukas Cavigelli
- Luca Benini

date: "2020-09-14T00:00:00Z"
doi: "10.1109/SMARTCOMP50058.2020.00065"

# Schedule page publish date (NOT publication's date).
publishDate: "2021-07-03T00:00:00Z"

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ["1"]

# Publication name and optional abbreviated publication name.
publication: In *2020 IEEE International Conference on Smart Computing*
publication_short: In *SMARTCOMP'20*

abstract: Motor-Imagery Brain-Machine Interfaces (MI-BMIs) promise direct and accessible communication between human brains and machines by analyzing brain activities recorded with Electroencephalography (EEG). Latency, reliability, and privacy constraints make it unsuitable to offload the computation to the cloud. Practical use cases demand a wearable, battery-operated device with low average power consumption for longterm use. Recently, sophisticated algorithms, in particular deep learning models, have emerged for classifying EEG signals. While reaching outstanding accuracy, these models often exceed the limitations of edge devices due to their memory and computational requirements. In this paper, we demonstrate algorithmic and implementation optimizations for EEGNET, a compact Convolutional Neural Network (CNN) suitable for many BMI paradigms. We quantize weights and activations to 8-bit fixed-point with a negligible accuracy loss of 0.4% on 4-class MI, and present an energy-efficient hardware-aware implementation on the Mr. Wolf parallel ultra-low power (PULP) System-on-Chip (SoC) by utilizing its custom RISC-VISA extensions and 8-core compute cluster. With our proposed optimization steps, we can obtain an overall speedup of 64 × and a reduction of up to 85% in memory footprint with respect to a single-core layer-wise baseline implementation. Our implementation takes only 5.82 ms and consumes 0.627 mJ per inference. With 21.0 GMAC/s/W, it is 256× more energy-efficient than an EEGNET implementation on an ARM Cortex-M7 (0.082 GMAC/s/W).

# Summary. An optional shortened abstract.
summary: Q-EEGNET is an energy-efficient implementation of EEGNET, a compact Convolutional Neural Network suitable for many BMI paradigms. Our algorithmic and implementation optimizations improve energy efficiency by more than 250 times.

tags: 
- Brain-machine interface
- Edge computing
- Parallel computing
- Machine learning
- Deep learning
- motor imagery

# Display this page in the Featured widget?
featured: false

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: 'q-eegnet.pdf'
url_code: 'https://github.com/pulp-platform/q-eegnet'
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
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
projects: []

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: ""
---
