# ATR-UMOD
The datastet in "Fusion Meets Diverse Conditions: A High-diversity Benchmark and Baseline for UAV-based Multimodal Object Detection with Condition Cues". The corresponding paper has been accepted in ICCV 2025.
# Abstract
Unmanned aerial vehicles (UAV)-based object detection with visible (RGB) and infrared (IR) images facilitates robust around-the-clock detection, driven by advancements in deep learning techniques and the availability of high-quality dataset. However, the existing dataset struggles to fully capture real-world complexity for limited imaging conditions. To this end, we introduce a high-diversity dataset ATR-UMOD covering varying scenarios, spanning altitudes from 80m to 300m, angles from 0° to 75°, and all-day, all-year time variations in rich weather and illumination conditions. Moreover, each RGB-IR image pair is annotated with 6 condition attributes, offering valuable high-level contextual information. To meet the challenge raised by such diverse conditions, we propose a novel prompt-guided condition-aware dynamic fusion (PCDF) to adaptively reassign multimodal contributions by leveraging annotated condition cues. By encoding imaging conditions as text prompts, PCDF effectively models the relationship between conditions and multimodal contributions through a task-specific soft-gating transformation. A prompt-guided condition-decoupling module further ensures the availability in practice without condition annotations. Experiments on ATR-UMOD dataset reveal the effectiveness of PCDF.
# Dataset
![图3](https://github.com/user-attachments/assets/20679e73-8f60-497e-a086-3b93d932579f)
ATR-UMOD contains 13,355 well-aligned RGB-IR image pairs at $640\times 512$ resolution, covering 161,799 RGB objects and 162,253 IR objects across car, SUV, van, bus, freight car, truck, motorcycle, trailer, excavator, crane, and tank truck categories.
It is divided into training and testing sets with 11,852 and 1,503 image pairs, respectively. 
To ensure rigorous evaluation, the subsets are derived from non-overlapping scenarios. Additionally, the object distribution across each subset has been carefully balanced to minimize data bias.

Our dataset is built spanning diverse imaging conditions in flying altitude, camera angle, shooting time, weather, illumination and scenario. Due to hardware limitations, raw RGB-IR images suffer from inevitable cross-modal misalignment for differences in imaging space and time. To this end, we employed homography transformation and region cropping for spatial calibration and timestamp alignment for temporal calibration. For annotation, RGB and IR objects were labeled separately with oriented bounding boxes.

We further enriched ATR-UMOD with detailed condition annotations, offering essential context to address visual bottlenecks and facilitate in-depth analysis of conditional impact on multimodal fusion.
Specifically, we labeled 6 key condition attributes for each image pair: Altitude, Angle, Time, Weather, Illumination, and Scenario.

Some representative examples of high-diversity imaging conditions in the ATR-UMOD dataset are presented as follows：
<img width="3713" height="1828" alt="图1-5——small" src="https://github.com/user-attachments/assets/1253e98e-bbb7-4851-ae96-6b49d291de45" />
# Download
The datatset can be load from BaiduYun: 

链接: https://pan.baidu.com/s/1rZ7MG5mI8inuiinvTVMRRg?pwd=accd 提取码: accd

The detailed meanings of the values of each condition attribute in the XML file are provided in the given txt file.
# Code
The PCDF in this paper will be released soon.
# Citation
Please cite this paper if you want to use it in your work.

