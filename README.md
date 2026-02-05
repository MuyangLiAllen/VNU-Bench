# 🎬 VNU-Bench: A Benchmark for Multi-Source Multimodal News Video Understanding

<p align="center">
  🤗 <a href="https://huggingface.co/datasets/Balibata/VNU-Bench"><b>Dataset</b></a> &nbsp; | &nbsp;
  📄 <a href="https://arxiv.org/pdf/2601.03434"><b>Paper</b></a>
</p>

VNU-Bench is the **first benchmark designed for cross-source, cross-video multimodal news understanding**, where models must reason over **multiple news reports of the same real-world event** instead of analyzing videos in isolation.

The dataset contains **424 news groups**, **1,375 videos**, and **2,501 high-quality multiple-choice questions** spanning 10 reasoning types.

---

## 📂 Dataset Structure

The dataset can be downloaded from:  
👉 **https://huggingface.co/datasets/Balibata/VNU-Bench**

Each sample belongs to a **news group**, which contains:

- Multiple news videos from different outlets covering the **same event**
- Multi-source reasoning questions (T1–T10)

Example JSON entry:

```json
{
  "topic": "Biogen Alzheimer drug Leqembi sales uptake",
  "video_ids": [
    "bFrJpOVkp88",
    "YkIF2Jzh_mQ",
    "t7hbNuIxZto"
  ],
  "qa": [
    {
      "task_id": "T1",
      "question": "...",
      "options": {
        "A": "...",
        "B": "...",
        "C": "...",
        "D": "..."
      },
      "correct_answer": "A"
    }
  ]
}

```

## 🎥 How to Access Original News Videos

You are able to locate the original videos in the following way. Or you can directly use videos attached in huggingface as well.

```
https://www.youtube.com/watch?v=VIDEO_ID
```

**Example**
```
video_id = bFrJpOVkp88
→ https://www.youtube.com/watch?v=bFrJpOVkp88
```
