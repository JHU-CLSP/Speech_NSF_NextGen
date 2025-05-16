---
title: Next Generation Tools for Spoken Language Science & Technology
layout: default
---

# 🔹 Introduction

<p align="center">
  <a href="https://github.com/k2-fsa/icefall">
    <img src="https://github.com/user-attachments/assets/925352f5-ffe9-4f33-873f-c8851a7b0ddb" alt="Icefall" width="100"/>
  </a>
  <a href="https://github.com/k2-fsa/k2">
    <img src="https://github.com/user-attachments/assets/d31f899e-3b76-462a-b516-6d8f44978347" alt="K2" width="100"/>
  </a>
  <a href="https://github.com/lhotse-speech/lhotse">  
    <img src="https://github.com/user-attachments/assets/756c82a2-b7f3-4a90-ae21-ca754fd90fbf" alt="Lhotse" width="100"/>
  </a>
</p>



The Kaldi open-source toolkit, developed in 2009 for automatic speech recognition (ASR), has played a foundational role in speech technology research. Its evolution continued in 2021 with the emergence of a follow-up trilogy—Icefall, k2, and Lhotse—demonstrating the rapid pace of innovation in speech algorithms and system design.

In response to the transformative changes in the field—such as the rise of large language models (LLMs), platforms like Hugging Face, and robust deep learning frameworks like PyTorch—this project aims to reimagine and modernize Kaldi’s capabilities to meet the emerging needs of the speech research community.

The primary objective of k2 is to re-implement all core functions of Kaldi natively in generic AI/deep learning frameworks, with a focus on PyTorch. This allows the seamless integration of cutting-edge developments in deep learning (e.g., novel optimization algorithms) into speech recognition research. The primary goals of Lhotse and Icefall include delivering efficient, user-friendly tools for data preparation, recipe development, and training modern ASR models.

**GitHub statistics for Lhotse, Icefall, and k2**  
<sup>*Within the last month (as of May 16, 2025)</sup>

<table>
  <thead>
    <tr>
      <th>GitHub Statistic</th>
      <th>Lhotse</th>
      <th>Icefall</th>
      <th>k2</th>
    </tr>
  </thead>
  <tbody>
    <tr><td>Watch</td><td>42</td><td>49</td><td>73</td></tr>
    <tr><td>Fork</td><td>233</td><td>337</td><td>224</td></tr>
    <tr><td>Star</td><td>1k</td><td>1.1k</td><td>1.2k</td></tr>
    <tr><td>Dependent repositories</td><td>252</td><td>0</td><td>49</td></tr>
    <tr><td>Merged PR<sup>*</sup></td><td>5</td><td>5</td><td>1</td></tr>
    <tr><td>Open PR<sup>*</sup></td><td>0</td><td>3</td><td>0</td></tr>
    <tr><td>Closed issues<sup>*</sup></td><td>1</td><td>14</td><td>0</td></tr>
    <tr><td>New issues<sup>*</sup></td><td>3</td><td>4</td><td>0</td></tr>
    <tr><td>Commits to master<sup>*</sup></td><td>7</td><td>5</td><td>1</td></tr>
    <tr><td>Additions<sup>*</sup></td><td>687</td><td>79</td><td>618</td></tr>
    <tr><td>Deletions<sup>*</sup></td><td>219</td><td>170</td><td>138</td></tr>
  </tbody>
</table>



#### Acknowledgments:

[<img src="https://github.com/user-attachments/assets/d5796c3a-bf9c-4876-b1fe-d49689f8b133" alt="NSF Official Logo" width="50"/>](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2120435&HistoricalAwards=false)
 This project was supported by U.S. National Science Foundation Award Number:2120435, NSF-CCRI project: CCRI: ENS: Next Generation Tools for Spoken Language Science & Technology. 


# 🔹 Projects

<p align="center">
  <a href="https://github.com/lhotse-speech/lhotse">  
    <img src="https://github.com/user-attachments/assets/756c82a2-b7f3-4a90-ae21-ca754fd90fbf" alt="Lhotse" width="200"/>
  </a>
</p>

Lhotse develops a modern approach to speech data preparation. Its design is inspired by data libraries commonly used in the ML community, such as pandas. Lhotse's philosophy may be summarized as *"simple things should be simple, complex things should be possible."* 

### 🎨 JHU Contributors

- **\#1** Piotr Żelasko — [1,221 commits](https://github.com/lhotse-speech/lhotse/commits?author=pzelasko) 🟩 110,336 ++ 🔴 43,656 --
- **\#2** Desh Raj — [248 commits](https://github.com/lhotse-speech/lhotse/commits?author=desh2608) 🟩 29,279 ++ 🔴 12,783 --
- **\#4** Jan (Yenda) Trmal — [33 commits](https://github.com/lhotse-speech/lhotse/commits?author=jtrmal) 🟩 2,093 ++ 🔴 651 --
- **\#6** Amir Hussein — [28 commits](https://github.com/lhotse-speech/lhotse/commits?author=AmirHussein96) 🟩 2,747 ++ 🔴 1,766 --
- **\#13** Matthew Wiesner — [13 commits](https://github.com/lhotse-speech/lhotse/commits?author=AmirHussein96) 🟩 3,425 ++ 🔴 627 --
- **\#24** Yiming Wang — [7 commits](https://github.com/lhotse-speech/lhotse/commits?author=freewym) 🟩 215 ++ 🔴 37 --
- **\#39** Dominik Klement — [2 commits](https://github.com/lhotse-speech/lhotse/commits?author=domklement) 🟩 1,602 ++ 🔴 0 --
- **\#53** Matthew Maciejewski — [1 commit](https://github.com/lhotse-speech/lhotse/commits?author=mmaciej2) 🟩 1,217 ++ 🔴 0 --
- **\#74** Henry Li Xinyuan — [1 commit](https://github.com/lhotse-speech/lhotse/commits?author=HSTEHSTEHSTE) 🟩 146 ++ 🔴 0 --
- **\#76** Dongji Gao — [1 commit](https://github.com/lhotse-speech/lhotse/commits?author=DongjiGao) 🟩 5 ++ 🔴 3 --

---

### 🎨 GPU-accelerated Guided Source Separation  
*by [Desh Raj](https://desh2608.github.io/)*

An improved implementation of [GSS](https://github.com/desh2608/gss) that leverages GPU-based pipelines — including batched frequency and segment processing — to perform detailed ablation studies on multiple parameters. Includes reproducible pipelines for speaker-attributed transcription on **LibriCSS**, **AMI**, and **AliMeeting** benchmarks.




### 🎨 Lhotse recipes

- [recipes/aishell3.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/aishell3.py) speech/asr
- [recipes/atcosim.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/atcosim.py) speech/asr
- [recipes/but_reverb_db.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/but_reverb_db.py)  reverberation database
- [recipes/chime6.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/chime6.py) speech/asr
- [recipes/csj.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/csj.py) speech/asr
- [recipes/cmu_kids.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/cmu_kids.py) speech/asr
- [recipes/dipco.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/dipco.py) speech/asr
- [recipes/edacc.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/edacc.py) speech/asr
- [recipes/gigast.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/gigaspeech.py) speech-translation
- [recipes/himia.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/himia.py) speaker-verification
- [recipes/librilight.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/librilight.py) speech/asr
- [recipes/must_c.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/must_c.py) speech-translation
- [recipes/speechcommands.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/speechcommands.py) speech/hotword-detection
- [recipes/uwb_atcc.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/uwb_atcc.py) speech/asr
- [recipes/xbmu_amdo31.py](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/xbmu_amdo31.py) speech/asr


- [Fleurs](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/fleurs.py) speech/language-id
- [radio stations](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/radio.py) speech/asr speech/language-id database 
- [SBCASE](https://github.com/lhotse-speech/lhotse/blob/master/lhotse/recipes/sbcsae.py) speech/diarization database

---

<p align="center">
  <a href="https://github.com/k2-fsa/icefall">
    <img src="https://github.com/user-attachments/assets/925352f5-ffe9-4f33-873f-c8851a7b0ddb" alt="Icefall" width="200"/>
  </a>
</p>

Icefall is the project where K2 and Lhotse ''meet''. It provides the speech and language research community a comprehensive collection of recipes for training modern speech processing systems on most of the popular speech data sets.

### 🎨 JHU Contributors
- **#11** Piotr Żelasko, [18 commits](https://github.com/k2-fsa/icefall/commits?author=pzelasko) 🟩 993 ++ 🔴 838 --
- **#15** Ruizhe Huang, [7 commits](https://github.com/k2-fsa/icefall/commits?author=huangruizhe) 🟩 95 ++ 🔴 74 --
- **#38** Dongji Gao, [2 commits](https://github.com/k2-fsa/icefall/commits?author=DongjiGao) 🟩 9,565 ++ 🔴 9 --
- **#43** Henry Li Xinyuan, [1 commit](https://github.com/k2-fsa/icefall/commits?author=HSTEHSTEHSTE) 🟩 2,124 ++ 🔴 3 --
- **#67** Amir Hussein, [1 commit](https://github.com/k2-fsa/icefall/commits?author=AmirHussein96) 🟩 6,114 ++ 🔴 1 --
- **#100** Jan "yenda" Trmal, [1 commit](https://github.com/k2-fsa/icefall/commits?author=jtrmal) 🟩 1 ++ 🔴 1 --

### 🎨 External Contributors
- **#2** Dan Povey, [200 commits](https://github.com/k2-fsa/icefall/commits?author=danpovey) 🟩 13,323 ++ 🔴 4,485 --

### 🎨 Continuous Streaming Multi-Talker ASR (by [Desh Raj](https://desh2608.github.io/))
[We investigated](https://arxiv.org/abs/2109.08555) Streaming Unmixing and Recognition Transducer (SURT) for continuous streaming multitalker ASR, and demonstrated the effectiveness of dual-path LSTMs and Transformers for generalization to diverse session lengths (recipes for the [LibriCSS](https://github.com/k2-fsa/icefall/tree/master/egs/libricss/SURT), [AMI and ICSI](https://github.com/k2-fsa/icefall/tree/master/egs/ami/SURT) datasets).

### 🎨 SPGISpeech (by [Desh Raj](https://desh2608.github.io/))
We developed an [Icefall recipe](https://github.com/k2-fsa/icefall/tree/master/egs/spgispeech/ASR) and trained models ([zipformer](https://huggingface.co/desh2608/icefall-asr-spgispeech-zipformer) and [stateless transducer](https://huggingface.co/desh2608/icefall-asr-spgispeech-pruned-transducer-stateless2)) for [SPGISpeech](https://arxiv.org/abs/2104.02014).

### 🎨 MGB-2 (by [Amir Hussein](https://github.com/AmirHussein96))
We developed an [Icefall recipe](https://github.com/k2-fsa/icefall/tree/master/egs/mgb2/ASR) and trained a model ([conformer-ctc](https://huggingface.co/AmirHussein/icefall-asr-mgb2-conformer_ctc-2022-27-06)) for [MGB-2](https://ieeexplore.ieee.org/abstract/document/7846277).

### 🎨 Contextual ASR (by Ruizhe Huang, Mahsa Yarmohammadi)
Developed recipes for Contextual ASR using the [ConEC dataset](https://github.com/huangruizhe/ConEC), and improved neural biasing ([PR](https://github.com/k2-fsa/icefall/pull/1763)).

### 🎨 Omni-temporal Classification (OTC) (by Dongji Gao, Paola Garcia, [Matthew Wiesner](https://m-wiesner.github.io/))
Proposed [OTC](https://ieeexplore.ieee.org/abstract/document/10389684) for learning from weak supervision:
- [BPE version](https://github.com/k2-fsa/icefall/blob/master/icefall/otc_graph_compiler.py)
- [Phone version](https://github.com/k2-fsa/icefall/blob/master/icefall/otc_phone_graph_compiler.py)

### 🎨 ASR + LID (by [Amir Hussein](https://github.com/AmirHussein96), Paola Garcia, [Matthew Wiesner](https://m-wiesner.github.io/))
Multitask ASR + Language ID model tested on multilingual and code-switched sets ([PR](https://github.com/k2-fsa/icefall/pull/1582)).

### 🎨 Other recipes
- [Kneser-Ney LM](https://github.com/k2-fsa/icefall/blob/e79833aad278f09792deceab5962b09ae4f56378/icefall/shared/make_kn_lm.py)
- [Librispeech](https://github.com/k2-fsa/icefall/tree/e79833aad278f09792deceab5962b09ae4f56378/egs/librispeech)
- [Fluent Speech Commands](https://github.com/k2-fsa/icefall/tree/master/egs/fluent_speech_commands/SLU)
- [Geolocation](https://github.com/geolocation-from-speech/icefall/tree/geolocation/egs/radio/geolocation)

---

<p align="center">
  <a href="https://github.com/k2-fsa/k2">
    <img src="https://github.com/user-attachments/assets/d31f899e-3b76-462a-b516-6d8f44978347" alt="K2" width="200"/>
  </a>
</p>

K2 brings FSA data structures into deep learning with GPU/CPU efficiency, PyTorch integration, and full autograd support.

### 🎨 JHU Contributors
- **#12** Piotr Żelasko, [4 commits](https://github.com/k2-fsa/k2/commits?author=pzelasko) 🟩 9,458 ++ 🔴 276 --
- **#13** Jan "yenda" Trmal, [4 commits](https://github.com/k2-fsa/k2/commits?author=jtrmal) 🟩 9,314 ++ 🔴 267 --
- **#15** Yiming Wang, [3 commits](https://github.com/k2-fsa/k2/commits?author=freewym) 🟩 234 ++ 🔴 67 --
- **#20** Desh Raj, [2 commits](https://github.com/k2-fsa/k2/commits?author=desh2608) 🟩 435 ++ 🔴 29 --
- **#27** Mahsa Yarmohammadi, [2 commits](https://github.com/k2-fsa/k2/commits?author=mahsa7823) 🟩 169 ++ 🔴 51 --
- **#35** Dongji Gao, [1 commit](https://github.com/k2-fsa/k2/commits?author=DongjiGao) 🟩 27 ++ 🔴 10 --

### 🎨 External Contributors
- **#2** Dan Povey, [214 commits](https://github.com/k2-fsa/k2/commits?author=danpovey) 🟩 73,771 ++ 🔴 30,586 --

### 🎨 k2 codes
- [Longest Common Prefix](https://github.com/k2-fsa/k2/pull/804)
- [Hybrid Autoregressive Transducer (HAT)](https://github.com/k2-fsa/k2/pull/1244)

---

# 🔹 Other projects

<p align="center">
  <img src="https://github.com/user-attachments/assets/08509f16-39f3-47ef-9093-183fa23a9499" alt="Other" width="200"/>
</p>

### 🎨 <img src="https://github.com/user-attachments/assets/5865aeaa-80c8-470f-bd96-38407f6405fb" width="80"/>

The [CHiME 8](https://www.chimechallenge.org/challenges/chime8/task1/index#tracks) submission relied on Lhotse and Whisper:
- [Data prep](https://github.com/chimechallenge/chime-utils?tab=readme-ov-file#data-preparation)
- [Usage](https://github.com/chimechallenge/chime-utils?tab=readme-ov-file#usage)
- [Manifest prep](https://github.com/chimechallenge/chime-utils/blob/main/DATAPREP.md) (Dipco, mixer6, notsofar1, CHiME6)

### 🎨 Target Speaker ASR with Whisper (by Dominik Klement, [Matthew Wiesner](https://m-wiesner.github.io/))
- [Repo](https://github.com/BUTSpeechFIT/TS-ASR-Whisper/tree/main)
- [Target Speaker Whisper](https://arxiv.org/pdf/2409.09543)
- [DiCoW](https://arxiv.org/pdf/2501.00114)
- [Data prep](https://github.com/BUTSpeechFIT/TS-ASR-Whisper/tree/main/scripts/data)

### 🎨 Hugging Face <img src="https://github.com/user-attachments/assets/9cca2970-4ff2-4847-b376-efda1bc17cec" width="25"/>
[k2-fsa](https://huggingface.co/k2-fsa) on Hugging Face:
- 1 dataset (LibriSpeech)
- 18 models
- 30 HF Spaces (ASR, TTS, tagging, LID)

---
