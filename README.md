# 🌉 Aligned Video Captions: Bridging Videos and LLMs for Efficient Retrieval-Augmented Generation

*Compact, modality-rich captions for scalable, agentic video understanding in RAG pipelines*

**Video-Enriched Retrieval Augmented Generation Using Aligned Video Captions** [[Paper](https://kevindelarosa.com/www2025-agent4ir_authorversion.pdf)] <br>
[Kevin Dela Rosa](https://kevindelarosa.com/) [<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/brands/twitter.svg" width="14" height="14">](https://twitter.com/kdrwins) [<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/brands/linkedin-in.svg" width="14" height="14">](https://www.linkedin.com/in/kdrosa/) [<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/brands/github.svg" width="14" height="14">](https://github.com/kdr) [<img src="https://raw.githubusercontent.com/FortAwesome/Font-Awesome/6.x/svgs/solid/graduation-cap.svg" width="14" height="14">](https://scholar.google.com/citations?user=8Pc5MiUAAAAJ&hl=en)

Stay tuned for follow up works using this dataset and future extensions.

## Releases

- [2025/04/28] 🎞️ **Video-Enriched Retrieval Augmented Generation Using Aligned Video Captions** accepted to [Agent4IR](https://sites.google.com/view/ai4ir/www-2025) at [ACM WWW 2025](https://www2025.thewebconf.org/), to appear in companion proceedings.
- [2024/07/18] [Early version](https://docs.google.com/presentation/d/105fSXZY7yPy7c8Iyc-LYOnGAs2pOKdAUptzHSqj2s5g/edit?slide=id.p#slide=id.p) of work presented at [Multimodal Representation and Retrieval](https://mrr-workshop.github.io/) at [SIGIR 2024](https://sigir-2024.github.io/index.html)

## Datasets

### Original Aligned Video Captions Dataset

The following are datasets artifacts supporting the 🎞️ **Video-Enriched Retrieval Augmented Generation Using Aligned Video Captions** publication.

We curated a dataset based on public youtube videos sampled from [Panda-70M](https://snap-research.github.io/Panda-70M/), which contains individual clip segments and a general visual scene caption learned from a set of open source video captioning models. Specifically we sampled roughly 2,000 videos from each of 15 top level YouTube categories, resulting in a dataset of 29,259 videos (1.5M video clips and corresponding visual captions) or roughly 215 days of footage. We then augmented that dataset with video subtitles gathered from the source videos and created the aligned transcripts.

**Statistics for Aligned Video Caption Dataset**

| **DATASET DIMENSION**     | **TOTAL**    | **MEDIAN**  |
|---------------------------|--------------|-------------|
| Video Count               | 29,259       | -           |
| Scene Count               | 1,476,462    | 31.00       |
| Video Duration (seconds)  | 18,584,396   | 478.00      |
|                           |              |             |
| **Text Character Length** |              |             |
|                           |              |             |
| Title                     | 1,548,810    | 51.00       |
| Description               | 30,565,705   | 780.00      |
| Title + Description       | 32,114,515   | 833.00      |
| Visual Video Captions     | 96,888,187   | 2,016.00    |
| Subtitles / ASR           | 141,926,062  | 3,472.00    |
| Aligned Captions          | 276,019,918  | 6,461.00    |

**Dataset Artifacts**

| Artifact                                       | Download                                                                                           |
|------------------------------------------------|----------------------------------------------------------------------------------------------------|
| Video Ids                                      | [link](https://drive.google.com/file/d/1L61XvG_dfBOHFl1gKhTb2SW_5f_3acF4/view?usp=sharing) (343KB) |
| Aligned Video Captions + Limited Metadata      | [link](https://drive.google.com/file/d/1tWLYMIRfge7l3oQ55Fyi8Q5toWxhGvby/view?usp=sharing) (602MB) |
| Generated Questions from RAG feasibility Study | [link](https://drive.google.com/file/d/1DsITfhk2AVOWnwOywGUKmP0gXWbDnOjq/view?usp=sharing) (252KB) |

If you wish to download the original videos and full video metadata, follow instructions from [here](https://github.com/snap-research/Panda-70M/tree/main/dataset_dataloading). The ChatGPT prompts used for generating video summaries, questions, and automatic judging are provided in [prompts](www2025/prompts/LLM_PROMPTS.xlsx) folder.


## Citation

If you find Aligned Video Captions useful for your research and applications, please cite using this BibTeX:

```bibtex
@inproceedings{10.1145/3701716.3716890,
  author       = {Dela Rosa, Kevin},
  title        = {Video-Enriched Retrieval Augmented Generation Using Aligned Video Captions},
  year         = {2025},
  isbn         = {9798400713316},
  publisher    = {Association for Computing Machinery},
  address      = {New York, NY, USA},
  url          = {https://doi.org/10.1145/3701716.3716890},
  doi          = {10.1145/3701716.3716890},
  booktitle    = {Companion Proceedings of the ACM Web Conference 2025},
  numpages     = {5},
  keywords     = {Multimodal Retrieval, Chatbots, Agentic Information Retrieval},
  location     = {Sydney, NSW, Australia},
  series       = {WWW '25}
}
```

