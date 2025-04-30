---
title: 'Evaluating the Impact of Adding Gaussian Noise as Data Augmentation on Electronic Nose for Black Tea Quality Classification'

# Authors
# If you created a profile for a user (e.g. the default `admin` user), write the username (folder name) here
# and it will be replaced with their full name and linked to their profile.
authors:
  - admin

# Author notes (optional)

date: '2024-01-15T00:00:00Z'
doi: ''

# Disable the citation button for this publication
share: false

# Schedule page publish date (NOT publication's date).
#publishDate: '2017-01-01T00:00:00Z'

# Publication type.
# Accepts a single type but formatted as a YAML list (for Hugo requirements).
# Enter a publication type from the CSL standard.
publication_types: ['paper-conference']

# Publication name and optional abbreviated publication name.
#publication: In *Hugo Blox Builder Conference*
#publication_short: In *ICW*

abstract: This study aims to evaluate whether the addition of Gaussian noise as data augmentation enhances the learning  process or merely introduces irrelevant data ("noise") into the system. The evaluation focuses on how the augmented data affects learning outcomes, particularly in scenarios with increasing noise levels. The study also compares classification performance with and without noise augmentation to assess its impact on model generalization and accuracy. Gaussian noise was applied at six controlled variance levels (0.01 to 0.3), and its influence on classification was analyzed across 1D-CNN and 2DCNN. Statistical analyses using MANOVA and the Kolmogorov Smirnov test confirmed that Gaussian noise augmentation preserved the core structure of the original data at lower noise levels while introducing realistic variability. The results show that for 1D-CNN, Zhou’s architecture consistently achieved 96% accuracy across all noise levels, indicating robustness to added noise. In contrast, 2D-CNN models, particularly ResNet34 with transfer learning, demonstrated exceptional performance at low noise levels (0.01) with an accuracy of 98.66%, but experienced a gradual performance decline as noise levels increased. This research provides insights into the effectiveness of Gaussian noise augmentation for improving model learning and highlights its limitations at higher noise levels. By comparing results with and without noise augmentation, the study demonstrates the importance of noise calibration to maintain the balance between variability and data integrity in classification tasks. 

# Summary. An optional shortened abstract.
summary: This study evaluates the effectiveness of Gaussian noise as data augmentation for electronic nose data in black tea quality classification, analyzing its impact on 1D-CNN and 2D-CNN model performance across different noise levels.

tags:
  - Deep learning model
  - AI
  - Vision
  - Signal processing
  - Electronic nose

# Display this page in the Featured widget?
featured: true

# Custom links (uncomment lines below)
# links:
# - name: Custom Link
#   url: http://example.org

url_pdf: ''
url_code: ''
url_dataset: ''
url_poster: 'poster.png'
url_project: ''
url_slides: '/slides/gaussian/'
url_source: ''
url_video: ''

# Featured image
# To use, add an image named `featured.jpg/png` to your page's folder.
image:
  caption: 'Image credit: [**Unsplash**](https://unsplash.com/photos/pLCdAaMFLTE)'
  focal_point: ''
  preview_only: false

# Associated Projects (optional).
#   Associate this publication with one or more of your projects.
#   Simply enter your project's folder or file name without extension.
#   E.g. `internal-project` references `content/project/internal-project/index.md`.
#   Otherwise, set `projects: []`.
projects:
  - "thesis project"

# Slides (optional).
#   Associate this publication with Markdown slides.
#   Simply enter your slide deck's filename without extension.
#   E.g. `slides: "example"` references `content/slides/example/index.md`.
#   Otherwise, set `slides: ""`.
slides: gaussian
---

## Document Viewers

### PDF Document {#pdf-viewer}

{{< view-document "/publication/conference-paper/conference-paper.pdf" "pdf" >}}

### PowerPoint Presentation {#ppt-viewer}

{{< view-document "/publication/conference-paper/paper-tesis.pptx" "ppt" >}}

