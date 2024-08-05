# Rethinking Image Editing Detection in the Era of Generative AI Revolution

The Generative Regional Editing (GRE) dataset was proposed in the [MM2024](https://2024.acmmm.org/) paper "Rethinking Image Editing Detection in the Era of Generative AI Revolution".

## Dataset

### Introduction
Considering copyright issues, the GRE dataset only provides edited images. The original images were collected from datasets such as COCO, Flickr2k, and VisualNews, as detailed in _**Section 3.1 Original Image Collection**_ of the paper.

Information and labels related to generative editing methods are included in the file name _xxxxxxxxxxxx.jpg_. The parsing code is as follows:
```python
file_name = '010502003a25.jpg'
edit_method_tag = int(file_name[2:4])

edit_method_dict = {
    1: 'GAN-MAT',
    2: 'GAN-LaMa',
    3: 'SD-Stable Diffusion V2.0',
    4: 'SD-ControlNet',
    5: 'SD-PaintByExample',
    6: 'Software-PhotoShop',
    7: 'Online-Weibo',
    8: 'Online-X(Twitter)',
}
edit_method = edit_method_dict[edit_method_tag]
```

### Download
If you would like to access the GRE dataset, please fill out this [Google Form](https://docs.google.com/forms/d/e/1FAIpQLSdftKYe2P9jtZkooX4Z_y4Ql8jJZKYieCzWbT6Pf_rxhysYhA/viewform?usp=sf_link). The download link will be sent to you once the form is accepted.

## License and Citation
The GRE dataset is released only for academic research. Researchers from educational institutes are allowed to use this database freely for noncommercial purposes.

**Reference Format:**
```
@inproceedings{10.1145/3664647.3681445,
    author = {Sun, Zhihao and Fang, Haipeng and Cao, Juan and Zhao, Xinying and Wang, Danding},
    title = {Rethinking Image Editing Detection in the Era of Generative AI Revolution},
    year = {2024},
    publisher = {Association for Computing Machinery},
    address = {Melbourne, VIC, Australia},
    url = {https://doi.org/10.1145/3664647.3681445},
    doi = {10.1145/3664647.3681445},
    booktitle = {Proceedings of the 32nd ACM International Conference on Multimedia},
    series = {MM '24}
}
```
