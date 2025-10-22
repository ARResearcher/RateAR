# RateAR Dataset
This repository introduces **RateAR**, a dataset of 321 AR images and 112 AR videos collected from various platforms and scenarios. 

# Dataset
The samples of the RateAR dataset can be found in the dataset folder. The full RateAR dataset can be downloaded from [Hugging Face](https://huggingface.co/datasets/I3TDataset/RateAR/tree/main). The dataset follows the hierarchical file structure shown below:
```
dataset
└───rateAR_images
│   └───image_1.png
│   ...
└───rateAR_videos
│   └───video_1.png
│   ...
```

_Creation:_ The RateAR dataset comprises 321 AR images and 112 AR videos. Figure 1 presents representative AR examples from the RateAR, illustrating a range of quality levels across all visual factors. We collected AR samples with custom-built applications across diverse environments. Specifically, we selected 321 AR images from the DiverseAR+ dataset spanning variations in placement, size, and shadow, captured on AVP, Samsung Galaxy S25, Google Pixel7, and Microsoft HoloLens2 in research labs, reading rooms, bedrooms, living rooms, study rooms, kitchens, and medical settings. In addition, we recorded 112 AR videos exhibiting the same variations using a Meta Quest~3 in research-lab, bedroom, living-room, and basement settings.

_Details:_ Each image features a single virtual object selected from a total of 24 classes. These span a range of domains including: medical anatomies of a human body (e.g., eye, brain), dynamic, user-manipulable objects (e.g., basketball, football, glove), and stationary objects (e.g., chair, can, box, table, etc.). The dataset captures a diverse range of visual quality statuses across 3 factors, recognized as key dimensions of photorealistic coherence and user safety in AR: **shadow realism, placement plausibility, size appropriateness**.

_Human Subjective Quality Score Labeling:_ To obtain subjective visual quality scores, we asked 4 AR experts to rate three visual factors of each scene on a 5-point scale using the Absolute Category Rating (ACR). ACR is a standardized approach for subjective quality assessment in which participants assign discrete scores (e.g., from 1 = ``bad" to 5 = ``excellent"). Each of the 433 AR samples was rated by all 4 AR experts, resulting in a total of 5,196 ratings. The mean score across 4 ratings was used as the final rating for our evaluation, ensuring consistency. Annotators used a graphical user interface that displayed the AR samples, with rating buttons beneath the images. Comprehensive instructions, including examples of both good and poor quality for each factor, were provided prior to the detailed labeling session; these can be found in [user instruction.pdf](https://github.com/ARResearcher/RateAR/blob/main/user%20instruction.pdf).

<p align="center"><img width="600" alt="Representative AR examples from the RateAR dataset illustrating various quality levels across 3 visual factors." src="https://github.com/ARResearcher/RateAR/blob/main/RateAR_samples.png"></p>
<p align="center">Figure 1. Representative examples from the RateAR dataset illustrating various quality levels across 3 visual factors: (1) Shadow realism: Virtual basket rendered with no shadow (poor), a shadow in the opposite direction (slightly degraded), or a shadow aligned with the real shadow (good); (2) Placement plausibility: Virtual can that appears obviously detached (poor), slightly elevated (slightly degraded), or properly seated (good); (6) Size appropriateness: Virtual car depicted as obviously small (poor), slightly small (slightly degraded), or normal-sized (good).</p> 

# Acknowledgments

The contributors of the dataset are [Lin Duan](https://scholar.google.com/citations?user=3KGmyogAAAAJ&hl=en), Eli Rotondo, Yanming Xiu, Sarah Eom, and [Maria Gorlatova](https://maria.gorlatova.com/bio/). For questions on this repository or the related paper, please contact Lin Duan at ld213 [AT] duke [DOT] edu.
