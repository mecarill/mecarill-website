---
title: '2PCNet: Two-Phase Consistency Training for Day-to-Night Unsupervised Domain Adaptive Object'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin
  - Wang Jian-Gang
  - Bharadwaj Veeravalli
  - Robby Tan

# Author notes (optional)
#author_notes:
#  - 'Equal contribution'
#  - 'Equal contribution'

date: '2023-07-01T00:00:00Z'
doi: ''

# Schedule page publish date (NOT publication's date).
publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Legend: 0 = Uncategorized; 1 = Conference paper; 2 = Journal article;
# 3 = Preprint / Working Paper; 4 = Report; 5 = Book; 6 = Book section;
# 7 = Thesis; 8 = Patent
publication_types: ['1']

# Publication name and optional abbreviated publication name.
publication:  The Conference on Computer Vision and Pattern Recognition (CVPR) 2023
publication_short: CVPR (2023)

abstract: Object detection at night is a challenging problem, particularly when the night image annotations are not assumed to be available. A few domain adaptation methods attempt to address the problem, and achieve state-of-the-art results by using the student-teacher framework. Unfortunately, these methods still suffer from false-positive error propagation stemming from the teacher’s wrong predictions, particularly for small scale objects and objects in low-light regions. To address this problem, we present 2PCNet, a twophase consistency unsupervised domain adaptation (UDA) network for nighttime object detection. Our 2PCNet employs high-confidence bounding-box predictions from the teacher in the first phase, and appends them to the student’s region proposals to be reevaluated by the teacher in the second phase, ensuring a mix of high and low confidence pseudo-labels. Night images and pseudo-labels are further scaled-down when used as an input to the student. This allows the student to have stronger small-scale pseudo-labels from the teacher, since the teacher generates the predictions based on the original full-scale image. Moreover, to mitigate errors stemming from objects in low-light regions and other night related attributes, we propose NightAug, which provides random night specific augmentations to the labelled daytime images, so that they can be closer to night images. Night specific augmentations include the addition of glare, blur, and noise to mimic the conditions of night images. Experiments on the publicly available BDD100K and SHIFT datasets demonstrate that our method achieves superior results to the state-of-the-art (+20%) as well as supervised models trained directly on the target data.

# Summary. An optional shortened abstract.
summary: 

tags: []

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: ''
url_project: ''
url_slides: ''
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: ''
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.

#projects:
#  - example

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
#slides: example
---

<!-- Supplementary notes can be added here, including [code, math, and images](https://wowchemy.com/docs/writing-markdown-latex/). -->
