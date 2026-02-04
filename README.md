# 📰 VNU-Bench  
**A Benchmark for Multi-Source Multimodal News Video Understanding**

VNU-Bench is the **first benchmark designed for cross-source, cross-video multimodal news understanding**, where models must reason over **multiple news reports of the same real-world event** instead of analyzing videos in isolation.

It evaluates capabilities such as:

- Multi-source claim comparison  
- Cross-source evidence integration  
- Conflict detection  
- Temporal development tracking  
- Narrative reconstruction  
- Multi-video summarization  

The dataset contains **429 news groups**, **1,405 videos**, and **2,501 high-quality multiple-choice questions** spanning 10 reasoning types.

---

## 📂 Dataset Structure

Each sample belongs to a **news group**, which contains:

- Multiple news videos from different outlets covering the **same event**
- Transcripts  
- Selected key frames  
- Multi-source reasoning questions (T1–T10)

Example JSON entry:

```json
{
  "topic": "Biogen Alzheimer drug Leqembi sales uptake",
  "video_ids": [
    "bFrJpOVkp88",
    "YkIF2Jzh_mQ",
    "t7hbNuIxZto"
  ]
}
