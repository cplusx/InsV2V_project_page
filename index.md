---
layout: page
title: Instruct Vid2Vid
---

<h2 align="center">Consistent Video-to-Video Transfer Using Synthetic Dataset</h2>

![Teaser](figures/teaser.png)

## Abstract

We introduce a novel and efficient approach for text-based video-to-video editing that eliminates the need for resource-intensive per-video-per-model finetuning. At the core of our approach is a synthetic paired video dataset tailored for video-to-video transfer tasks. Inspired by Instruct Pix2Pix's image transfer via editing instruction, we adapt this paradigm to the video domain. Extending the Prompt-to-Prompt to videos, we efficiently generate paired samples, each with an input video and its edited counterpart. Alongside this, we introduce the Long Video Sampling Correction during sampling, ensuring consistent long videos across batches. Our method surpasses current methods like Tune-A-Video, heralding substantial progress in text-based video-to-video editing and suggesting exciting avenues for further exploration and deployment.

## Examples
<style>
    .gif-container {
        display: flex;
        flex-wrap: wrap;
    }

    .gif-item {
        flex: 1 1 calc(50% - 10px); /* Makes sure there are only 2 items per row with a gap of 10px */
        margin: 5px; /* This provides the gap */
    }
</style>

<div class="gif-container">
    {% for image in site.static_files %}
        {% if image.path contains 'videos/' and image.extname == '.gif' %}
            <div class="gif-item">
                <img src=".{{ image.path }}" alt="{{ image.name }}">
            </div>
        {% endif %}
    {% endfor %}
</div>



## BibTeX

```plaintext
@article{your_bib_key,
  title={Your Paper Title},
  author={Author1, Name1 and Author2, Name2},
  journal={Name of Journal/Conference},
  year={202x},
  volume={xx},
  number={x},
  pages={xx--xx},
  publisher={Publisher Name}
}

