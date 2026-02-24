# 🔹 Introduction
<p align="center">
  <a href="https://github.com/k2-fsa/icefall">
    <img src="https://github.com/user-attachments/assets/925352f5-ffe9-4f33-873f-c8851a7b0ddb" alt="Icefall" width="100"/>
  <a href="https://github.com/k2-fsa/k2">
    <img src="https://github.com/user-attachments/assets/d31f899e-3b76-462a-b516-6d8f44978347" alt="K2" width="100"/>
  <a href="https://github.com/lhotse-speech/lhotse">  
    <img src="https://github.com/user-attachments/assets/756c82a2-b7f3-4a90-ae21-ca754fd90fbf" alt="Lhotse" width="100"/>
</p>


The Kaldi open-source toolkit, developed in 2009 for automatic speech recognition (ASR), has played a foundational role in speech technology research. Its evolution continued in 2021 with the emergence of a follow-up trilogy—Icefall, k2, and Lhotse—demonstrating the rapid pace of innovation in speech algorithms and system design.

In response to the transformative changes in the field—such as the rise of large language models (LLMs), platforms like Hugging Face, and robust deep learning frameworks like PyTorch—this project aims to reimagine and modernize Kaldi’s capabilities to meet the emerging needs of the speech research community.

The primary objective of k2 is to re-implement all core functions of Kaldi natively in generic AI/deep learning frameworks, with a focus on PyTorch. This allows the seamless integration of cutting-edge developments in deep learning (e.g., novel optimization algorithms) into speech recognition research. The primary goals of Lhotse and Icefall include delivering efficient, user-friendly tools for data preparation, recipe development, and training modern ASR models.

<div align="center">

  GitHub statistics for Lhotse, Icefall, and k2. <sup>*</sup>within last month (as of September 30 2025)

| GitHub statistic        | Lhotse | Icefall | k2   |
|-------------------------|--------|---------|------|
| Watch                   | 42     | 50      | 72   |
| Fork                    | 251    | 375     | 230  |
| Star                    | 1.1k     | 1.2k    | 1.3k |
| Dependent repositories  | 316    | 0       | 57   |
| Merged PR<sup>*</sup>   | 12      | 4       | 0    |
| Open PR<sup>*</sup>     | 9      | 1       | 0    |
| Closed issue<sup>*</sup>| 2      | 6      | 0    |
| New issue<sup>*</sup>   | 2      | 5       | 0    |
| Commits to master<sup>*</sup>| 12      | 4       | 0    |
| Additions<sup>*</sup>   | 1,658    | 53,242      | 0  |
| Deletions<sup>*</sup>   | 70    | 8     | 0  |

</div>


#### Acknowledgments:

[<img src="https://github.com/user-attachments/assets/d5796c3a-bf9c-4876-b1fe-d49689f8b133" alt="NSF Official Logo" width="50"/>](https://www.nsf.gov/awardsearch/showAward?AWD_ID=2120435&HistoricalAwards=false)
 This project was supported by U.S. National Science Foundation Award Number:2120435, NSF-CCRI project: CCRI: ENS: Next Generation Tools for Spoken Language Science & Technology. 

# 🔹 Projects

<p align="center">
  <a href="https://github.com/lhotse-speech/lhotse">  
    <img src="https://github.com/user-attachments/assets/756c82a2-b7f3-4a90-ae21-ca754fd90fbf" alt="Lhotse" width="200"/>
</p>

Lhotse develops a modern approach to speech data preparation. Its design is inspired by data libraries commonly used in the ML community, such as pandas. Lhotse's philosophy may be summarized as ''simple things should be simple, complex things should be possible.'' 

### 🎨 JHU Contributors
- **\#1** Piotr Żelasko, [1,231 commits](https://github.com/lhotse-speech/lhotse/commits?author=pzelasko) 🟩 112,538 ++ 🔴 43,832 --
- **\#2** Desh Raj, [248 commits](https://github.com/lhotse-speech/lhotse/commits?author=desh2608) 🟩 29,279 ++ 🔴 12,783 --
- **\#4** Jan (Yenda) Trmal, [33 commits](https://github.com/lhotse-speech/lhotse/commits?author=jtrmal) 🟩 2,093 ++ 🔴 651 --
- **\#6** Amir Hussein, [28 commits](https://github.com/lhotse-speech/lhotse/commits?author=AmirHussein96) 🟩 2,747 ++ 🔴 1766 --
- **\#13** Matthew Wiesner, [13 commits](https://github.com/lhotse-speech/lhotse/commits?author=AmirHussein96) 🟩 3,425 ++ 🔴 627 --
- **\#23** Yiming Wang, [7 commits](https://github.com/lhotse-speech/lhotse/commits?author=freewym) 🟩 215 ++ 🔴 37 --
- **\#38** Dominik Klement, [2 commits](https://github.com/lhotse-speech/lhotse/commits?author=domklement) 🟩 1602 ++ 🔴 0 --
- **\#56** Matthew Maciejewski, [1 commit](https://github.com/lhotse-speech/lhotse/commits?author=mmaciej2) 🟩 1,217 ++ 🔴 0 --
- **\#76** Dongji Gao, [1 commit](https://github.com/lhotse-speech/lhotse/commits?author=DongjiGao) 🟩 5 ++ 🔴 3 --
- **\#83** Henry Li Xinyuan, [1 commit](https://github.com/lhotse-speech/lhotse/commits?author=HSTEHSTEHSTE) 🟩 146 ++ 🔴 0 --

### 🎨 GPU-accelerated Guided Source Separation (by [Desh Raj](https://desh2608.github.io/))
Improved implementation of [GSS](https://github.com/desh2608/gss) that leverages the power of modern GPU-based pipelines, such as batched processing of frequencies and segments. This allows us to perform detailed ablation studies over several parameters of the GSS algorithm. There are reproducible pipelines for speaker-attributed transcription of popular meeting benchmarks: LibriCSS, AMI, and AliMeeting.



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


_______________________________________________________________________________________

<p align="center">
  <a href="https://github.com/k2-fsa/icefall">
    <img src="https://github.com/user-attachments/assets/925352f5-ffe9-4f33-873f-c8851a7b0ddb" alt="Icefall" width="200"/>
</p>

Icefall is the project where K2 and Lhotse ''meet''. It provides the speech and language research community a comprehensive collection of recipes for training modern speech processing systems on most of the popular speech data sets.  

### 🎨 JHU Contributors
- **\#9** Desh Raj, [19 commits](https://github.com/k2-fsa/icefall/commits?author=desh2608) 🟩 39,142 ++ 🔴 22,339 --
- **\#10** Piotr Żelasko, [18 commits](https://github.com/k2-fsa/icefall/commits?author=pzelasko) 🟩 993 ++ 🔴 838 --
- **\#15** Ruizhe Huang, [7 commits](https://github.com/k2-fsa/icefall/commits?author=huangruizhe) 🟩 95 ++ 🔴 74 --
- **\#29** Amir Hussein, [3 commit](https://github.com/k2-fsa/icefall/commits?author=AmirHussein96) 🟩 59,348 ++ 🔴 2 --
- **\#31** Dongji Gao, [2 commits](https://github.com/k2-fsa/icefall/commits?author=DongjiGao) 🟩 9,565 ++ 🔴 9 --
- **\#44** Henry Li Xinyuan, [1 commit](https://github.com/k2-fsa/icefall/commits?author=HSTEHSTEHSTE) 🟩 2,124 ++ 🔴 3 --

### 🎨 External Contributors
- **\#2** Dan Povey, [200 commits](https://github.com/k2-fsa/icefall/commits?author=danpovey) 🟩 13,323 ++ 🔴 4,485 --

###  🎨 HENT-SRT (by [Amir Hussein](https://github.com/AmirHussein96), Paola Garcia, [Matthew Wiesner](https://m-wiesner.github.io/))
We introduced [HENT-SRT](https://arxiv.org/pdf/2506.02157) (Hierarchical Efficient Neural Transducer for Speech Recognition and Translation
), a novel hierarchical transducer architecture for joint speech recognition and translation (ST). HENT-SRT ([Icefall recipe](https://github.com/k2-fsa/icefall/tree/master/egs/multi_conv_zh_es_ta)) significantly outperforms previous state-ofthe-art transducer-based ST models and closes the gap with attention-based encoder-decoder architectures, while achieving superior ASR performance. Our approach offers substantial gains in streaming scenarios without introducing additional delays.

### 🎨 Continuous Streaming Multi-Talker ASR (by [Desh Raj](https://desh2608.github.io/))
[We investigated](https://arxiv.org/abs/2109.08555) Streaming Unmixing and Recognition Transducer (SURT) for continuous streaming multitalker ASR, and demonstrated the effectiveness of dual-path LSTMs and Transformers for generalization to diverse session lengths (recipes for the [LibriCSS](https://github.com/k2-fsa/icefall/tree/master/egs/libricss/SURT), [AMI and ICSI](https://github.com/k2-fsa/icefall/tree/master/egs/ami/SURT) datasets).

###  🎨 SPGISpeech (by [Desh Raj](https://desh2608.github.io/))
We developed an [Icefall recipe](https://github.com/k2-fsa/icefall/tree/master/egs/spgispeech/ASR) and trained models ([zipformer](https://huggingface.co/desh2608/icefall-asr-spgispeech-zipformer) and [stateless transducer](https://huggingface.co/desh2608/icefall-asr-spgispeech-pruned-transducer-stateless2) models on Hugging Face) for [SPGISpeech](https://arxiv.org/abs/2104.02014), a dataset consisting of 5,000 hours of recorded company earnings calls and their respective transcriptions.

###  🎨 MGB-2 (by [Amir Hussein](https://github.com/AmirHussein96))
We developed an [Icefall recipe](https://github.com/k2-fsa/icefall/tree/master/egs/mgb2/ASR) and trained a model ([conformer-ctc](https://huggingface.co/AmirHussein/icefall-asr-mgb2-conformer_ctc-2022-27-06) model on Hugging Face) for [Multi-Dialect Broadcast News Arabic Speech Recognition (MGB-2)](https://ieeexplore.ieee.org/abstract/document/7846277) challenge on Arabic multi-dialect broadcast media recognition.

###  🎨 Contextual ASR (by Ruizhe Huang, Mahsa Yarmohammadi)
Developed recipes for Contextual ASR. This is the process by which an ASR system is provided with contextual information derived from metadata associated with the audio, typically in the form of a list of words or phrases likely to be spoken, with the goal of improving the recognition accuracy of named entities and other infrequent terms. Our work on Contextual ASR is recognized for introducing the ConEC dataset ([ConEC](https://github.com/huangruizhe/ConEC)), followed by a method for improving neural biasing beyond shallow language model fusion ([Pull request - Neural Biasing](https://github.com/k2-fsa/icefall/pull/1763)).


### 🎨 Omni-temporal Classification (OTC) (by Dongji Gao, Paola Garcia, [Matthew Wiesner](https://m-wiesner.github.io/))
Training ASR systems requires large amounts of well-curated paired data. However, human annotators usually perform "non-verbatim" transcription, which can result in poorly trained models. We designed and implemented Omni-temporal Classification ([OTC](https://ieeexplore.ieee.org/abstract/document/10389684)), a novel training criterion that explicitly incorporates label uncertainties originating from such weak supervision. This allows the model to effectively learn speech-text alignments while accommodating errors present in the training transcripts ([OTC w/ BPE units](https://github.com/k2-fsa/icefall/blob/master/icefall/otc_graph_compiler.py), [OTC w/ phone units](https://github.com/k2-fsa/icefall/blob/master/icefall/otc_phone_graph_compiler.py)).

###  🎨 ASR + LID (by [Amir Hussein](https://github.com/AmirHussein96), Paola Garcia, [Matthew Wiesner](https://m-wiesner.github.io/))
Created a multitask learning framework that synchronizes Language Identification (LID) with ASR, utilizing a neural transducer architecture. We demonstrate the efficacy of our proposed approach on conversational multilingual (Arabic, Spanish, Mandarin) and CS (Spanish-English, Mandarin-English) test sets ([Pull request - ASR SEAME Recipe](https://github.com/k2-fsa/icefall/pull/1582)).

### 🎨 Other recipes

- [Kneser-Ney language model smoothing](https://github.com/k2-fsa/icefall/blob/e79833aad278f09792deceab5962b09ae4f56378/icefall/shared/make_kn_lm.py)
- [Librispeech](https://github.com/k2-fsa/icefall/tree/e79833aad278f09792deceab5962b09ae4f56378/egs/librispeech) - partial contribution
- [Fluent Speech Commands recipe](https://github.com/k2-fsa/icefall/tree/master/egs/fluent_speech_commands/SLU)
- Recipe for [Geolocation](https://github.com/geolocation-from-speech/icefall/tree/geolocation/egs/radio/geolocation) dataset using Lhotse and Icefall
- Dialectal IWSLT-Tunisian 2022 shared task ASR and ST [recipes](https://github.com/k2-fsa/icefall/tree/master/egs/iwslt22_ta)

_______________________________________________________________________________________
<p align="center">
  <a href="https://github.com/k2-fsa/k2">
    <img src="https://github.com/user-attachments/assets/d31f899e-3b76-462a-b516-6d8f44978347" alt="K2" width="200"/>
</p>

K2 brings data structures and algorithms from the field of finite state automata (FSA) into the world of deep learning. It provides efficient CPU and GPU implementations of commonly used FSA operations and integrates them seamlessly with PyTorch's tensor and automatic differentiation mechanisms, thus admitting - and benefiting from - the inner complexity of the speech recognition, instead of trying to remove it.
### 🎨 JHU Contributors
- **\#12** Piotr Żelasko, [4 commits](https://github.com/k2-fsa/k2/commits?author=pzelasko) 🟩 9,458 ++ 🔴 276 --
- **\#13** Jan "yenda" Trmal, [4 commits](https://github.com/k2-fsa/k2/commits?author=jtrmal) 🟩 9,314 ++ 🔴 267 --
- **\#16** Mahsa Yarmohammadi, [3 commits](https://github.com/k2-fsa/k2/commits?author=mahsa7823) 🟩 173 ++ 🔴 51 --
- **\#19** Yiming Wang, [3 commits](https://github.com/k2-fsa/k2/commits?author=freewym) 🟩 234 ++ 🔴 67 --
- **\#22** Desh Raj, [2 commits](https://github.com/k2-fsa/k2/commits?author=desh2608) 🟩 435 ++ 🔴 29 --
- **\#35** Dongji Gao, [1 commit](https://github.com/k2-fsa/k2/commits?author=DongjiGao) 🟩 27 ++ 🔴 10 --

### 🎨 External Contributors
- **\#2** Dan Povey, [214 commits](https://github.com/k2-fsa/k2/commits?author=danpovey) 🟩 73,771 ++ 🔴 30,586 --

### 🎨 k2 codes
- Test whether FSA is [acyclic](https://github.com/k2-fsa/k2/pull/26). 
- Fast parallel computation of longest common prefixes for eﬃcient pattern matching ([kmp-LCP](https://github.com/k2-fsa/k2/pull/804)).
- Implementation of the Hybrid Autoregressive Transducer loss ([HAT](https://github.com/k2-fsa/k2/pull/1244)).

_______________________________________________________________________________________
# 🔹 Other projects
<p align="center">
  <img src="https://github.com/user-attachments/assets/08509f16-39f3-47ef-9093-183fa23a9499", alt="Other" width="200"/>
</p>

### 🎨 <img src="https://github.com/user-attachments/assets/5865aeaa-80c8-470f-bd96-38407f6405fb" width="80"/>

The [CHiME 8](https://www.chimechallenge.org/challenges/chime8/task1/index#tracks) submission relied on Lhotse for data preparation, audio loading, data manipulation, and constructing the PyTorch dataloaders. Once in this format, it was possible to interface with standard Whisper training recipes in the [Whisper GitHub](https://github.com/openai/whisper) repo or on Hugging Face. 
- [Data preparation](https://github.com/chimechallenge/chime-utils?tab=readme-ov-file#data-preparation) for k2/Icefall and ESPNet.
- [Usage](https://github.com/chimechallenge/chime-utils?tab=readme-ov-file#usage) prepares CHiME-8 data lhotse manifests.
- [Manifest preparation for different toolkits](https://github.com/chimechallenge/chime-utils/blob/main/DATAPREP.md) (Datasets included: Dipco, mixer6, notsofar1, CHiME6).

### 🎨 Target Speaker ASR with Whisper (by [BUT](https://speech.fit.vut.cz/) in collaboration with Dominik Klement, [Matthew Wiesner](https://m-wiesner.github.io/))
The [repository](https://github.com/BUTSpeechFIT/TS-ASR-Whisper/tree/main) contains the official implementation of the following publications: [Target Speaker Whisper](https://arxiv.org/pdf/2409.09543) and [DiCoW](https://arxiv.org/pdf/2501.00114): Diarization-Conditioned Whisper for Target Speaker Automatic Speech Recognition. It relied on Lhotse for homogenizing the data preparation across various datasets, such as AMI, Librispeech.  This project is a collaboration between  Alex Polok and Lukás Burget from [BUT](https://speech.fit.vut.cz/) and Dominik Klement, [Matthew Wiesner](https://m-wiesner.github.io/)
- [Data preparation](https://github.com/BUTSpeechFIT/TS-ASR-Whisper/tree/main/scripts/data) (AMI, Librispeech, etc)

### 🎨 Long-Form Fuzzy Speech-to-Text Alignment for 1000+ Languages (by Ruizhe Huang)
Ruizhe has introduced a long-form fuzzy speech-to-text aligner built on Torchaudio that can align hours of audio with imperfect transcriptions (e.g., lectures, earnings calls, audiobooks). As part of the implementation, the aligner relies on WFSTs via k2 to allow skipping or reordering parts of the text during alignment. The library is provided open-source and can be used out-of-the-box with users’ models for efficient alignment and segmentation of raw audio recordings and transcripts. A [web demo](https://colab.research.google.com/drive/1WvGPqBHg_EyEPeiYSiPChvuF2M0nzx88) is also available on Google Colab, demonstrating alignment of earnings calls and audiobooks in different languages with minimal pre-processing.

### 🎨 Hugging Face <img src="https://github.com/user-attachments/assets/9cca2970-4ff2-4847-b376-efda1bc17cec" width="25"/>
Researchers and developers increasingly rely on the open-source platform Hugging Face for pre-trained models, datasets, and tools to efficiently build and deploy AI applications. [k2-fsa](https://huggingface.co/k2-fsa) is available on Hugging Face. As of now, it has published one dataset (LibriSpeech) and 18 models. Additionally, 30 HF Spaces have been released, offering inference APIs and demos for tasks such as speech recognition, text-to-speech, audio tagging, and spoken language identification using Next-gen Kaldi.

# 🔹 Publications
- **WST: Weakly Supervised Transducer for Automatic Speech Recognition**
   Dongji Gao, Chenda Liao, Changliang Liu, Matthew Wiesner, Leibny Paola García, Dan Povey, S. Khudanpur, Jian Wu
   arXiv.org 2025
   [open paper page](https://arxiv.org/pdf/2511.04035.pdf)
   <details>
     <summary> Abstract </summary>
     The Recurrent Neural Network-Transducer (RNN-T) is widely adopted in end-to-end (E2E) automatic speech recognition (ASR) tasks but depends heavily on large-scale, high-quality annotated data, which are often costly and difficult to obtain. To mitigate this reliance, we propose a Weakly Supervised Transducer (WST), which integrates a flexible training graph designed to robustly handle errors in the transcripts without requiring additional confidence estimation or auxiliary pre-trained models. Empirical evaluations on synthetic and industrial datasets reveal that WST effectively maintains performance even with transcription error rates of up to 70%, consistently outperforming existing Connectionist Temporal Classification (CTC)-based weakly supervised approaches, such as Bypass Temporal Classification (BTC) and Omni-Temporal Classification (OTC). These results demonstrate the practical utility and robustness of WST in realistic ASR settings. The implementation will be publicly available.
  </details>
  
- **Listening to Multi-talker Conversations: Modular and End-to-end Perspectives**
   Desh Raj
   arXiv.org 2024
   [open paper page](https://arxiv.org/pdf/2402.08932.pdf)
   <details>
     <summary> Abstract </summary>
     Since the first speech recognition systems were built more than 30 years ago, improvement in voice technology has enabled applications such as smart assistants and automated customer support. However, conversation intelligence of the future requires recognizing free-flowing multi-party conversations, which is a crucial and challenging component that still remains unsolved. In this dissertation, we focus on this problem of speaker-attributed multi-talker speech recognition, and propose two perspectives which result from its probabilistic formulation. In the modular perspective, we build a pipeline of sub-tasks involving speaker diarization, target speaker extraction, and speech recognition. Our first contribution is a method to perform overlap-aware diarization by reformulating spectral clustering as a constrained optimization problem. We also describe an algorithm to ensemble diarization outputs, either to combine overlap-aware systems or to perform multi-channel diarization by late fusion. Once speaker segments are identified, we robustly extract single-speaker utterances from the mixture using a GPU-accelerated implementation of guided source separation, which allows us to use an off-the-shelf ASR system to obtain speaker-attributed transcripts. Since the modular approach suffers from error propagation, we propose an alternate"end-to-end"perspective on the problem. For this, we describe the Streaming Unmixing and Recognition Transducer (SURT). We show how to train SURT models efficiently by carefully designing the network architecture, objective functions, and mixture simulation techniques. Finally, we add an auxiliary speaker branch to enable joint prediction of speaker labels synchronized with the speech tokens. We demonstrate that training on synthetic mixtures and adapting with real data helps these models transfer well for streaming transcription of real meeting sessions.
  </details>

- **Improving Neural Biasing for Contextual Speech Recognition by Early Context Injection and Text Perturbation**
   Ruizhe Huang, M. Yarmohammadi, S. Khudanpur, Dan Povey
   Interspeech 2024
   [open paper page](https://arxiv.org/pdf/2407.10303.pdf)
   <details>
     <summary> Abstract </summary>
     Existing research suggests that automatic speech recognition (ASR) models can benefit from additional contexts (e.g., contact lists, user specified vocabulary). Rare words and named entities can be better recognized with contexts. In this work, we propose two simple yet effective techniques to improve context-aware ASR models. First, we inject contexts into the encoders at an early stage instead of merely at their last layers. Second, to enforce the model to leverage the contexts during training, we perturb the reference transcription with alternative spellings so that the model learns to rely on the contexts to make correct predictions. On LibriSpeech, our techniques together reduce the rare word error rate by 60% and 25% relatively compared to no biasing and shallow fusion, making the new state-of-the-art performance. On SPGISpeech and a real-world dataset ConEC, our techniques also yield good improvements over the baselines.
  </details>
  
- **Where are you from? Geolocating Speech and Applications to Language Identification**
   P. Foley, Matthew Wiesner, B. Odoom, Leibny Paola Garcia Perera, Kenton Murray, Philipp Koehn
   North American Chapter of the Association for Computational Linguistics 2024
   [open paper page](https://www.aclanthology.org/2024.naacl-long.286.pdf)
   <details>
     <summary> Abstract </summary>
     We train models to answer the question, Where are you from? and show how such models can be repurposed for language identification (LID). To our knowledge, this paper is the first to introduce data sources, methods and models to tackle the task of geolocation of speech at a global scale, and the first to explore using geolocation as a proxy-task for LID. Specifically, we explore whether radio broadcasts with known origin can be used to train regression and classification-based models for geolocating speech. We build models on top of self-supervised pretrained models, using attention pooling to qualitatively verify that the model geolocates the speech itself, and not other channel artifacts.The best geolocation models localize speaker origin to around 650km. We confirm the value of speech geolocation as a proxy task by using speech geolocation models for zero-shot LID. Finally, we show that fine-tuning geolocation models for LID outperforms fine-tuning pretrained Wav2Vec2.0 models, and achieves state-of-the-art performance on the FLEURS benchmark.
  </details>

- **Updated corpora and benchmarks for long-form speech recognition**
   Jennifer Drexler Fox, D. Raj, N. Delworth, Q. McNamara, C. Miller, M. Jetté
   IEEE ICASSP 2024
   [open paper page](https://arxiv.org/pdf/2309.15013)
   <details>
     <summary> Abstract </summary>
     The vast majority of ASR research uses corpora in which both the training and test data have been pre-segmented into utterances. In most real-word ASR use-cases, however, test audio is not segmented, leading to a mismatch between inference-time conditions and models trained on segmented utterances. In this paper, we re-release three standard ASR corpora - TED-LIUM 3, Gigapeech, and VoxPopuli-en - with updated transcription and alignments to enable their use for long-form ASR research. We use these reconstituted corpora to study the train-test mismatch problem for transducers and attention-based encoder-decoders (AEDs), confirming that AEDs are more susceptible to this issue. Finally, we benchmark a simple long-form training for these models, showing its efficacy for model robustness under this domain shift.
  </details>


- **ConEC: Earnings Call Dataset with Real-world Contexts for Benchmarking Contextual Speech Recognition**
   Ruizhe Huang, M. Yarmohammadi, J. Trmal, Jing Liu, Desh Raj, Leibny Paola García, A. Ivanov, Patrick Ehlen, Mingzhi Yu, Dan Povey, S. Khudanpur
   International Conference on Language Resources and Evaluation 2024
   [open paper page](https://www.aclanthology.org/2024.lrec-main.328.pdf)
   <details>
     <summary> Abstract </summary>
     Knowing the particular context associated with a conversation can help improving the performance of an automatic speech recognition (ASR) system. For example, if we are provided with a list of in-context words or phrases — such as the speaker’s contacts or recent song playlists — during inference, we can bias the recognition process towards this list. There are many works addressing contextual ASR; however, there is few publicly available real benchmark for evaluation, making it difficult to compare different solutions. To this end, we provide a corpus (“ConEC”) and baselines to evaluate contextual ASR approaches, grounded on real-world applications. The ConEC corpus is based on public-domain earnings calls (ECs) and associated supplementary materials, such as presentation slides, earnings news release as well as a list of meeting participants’ names and affiliations. We demonstrate that such real contexts are noisier than artificially synthesized contexts that contain the ground truth, yet they still make great room for future improvement of contextual ASR technology.
  </details>

- **Enhancing Neural Transducer for Multilingual ASR with Synchronized Language Diarization**
   Amir Hussein, Desh Raj, Matthew Wiesner, Dan Povey, Paola Garcia, S. Khudanpur
   Interspeech 2024
   [open paper page](https://doi.org/10.21437/interspeech.2024-1418)
   <details>
     <summary> Abstract </summary>
     In multilingual environments, seamless language switching, including code-switching (CS) within utterances, is essential for real-time applications. Conventional Automatic Speech Recognition (ASR) combined with language diarization requires post-processing to synchronize language labels with recognized words accurately, presenting a considerable challenge. In this study, we introduce a multitask learning framework that synchronizes Language Identification (LID) with ASR, utilizing a neural transducer architecture. This auxiliary task integrates both acoustic and lexical features to perform LID. Furthermore, we use resulting language representation as an auxiliary input to improve ASR. We demonstrate the efficacy of our proposed approach on conversational multilingual (Arabic, Spanish, Mandarin) and CS (Spanish-English, Mandarin-English) test sets.
  </details>

- **On Speaker Attribution with SURT**
   Desh Raj, Matthew Wiesner, Matthew Maciejewski, Leibny Paola García-Perera, Daniel Povey, S. Khudanpur
   The Speaker and Language Recognition Workshop 2024
   [open paper page](https://arxiv.org/pdf/2401.15676.pdf)
   <details>
     <summary> Abstract </summary>
     The Streaming Unmixing and Recognition Transducer (SURT) has recently become a popular framework for continuous, streaming, multi-talker speech recognition (ASR). With advances in architecture, objectives, and mixture simulation methods, it was demonstrated that SURT can be an efficient streaming method for speaker-agnostic transcription of real meetings. In this work, we push this framework further by proposing methods to perform speaker-attributed transcription with SURT, for both short mixtures and long recordings. We achieve this by adding an auxiliary speaker branch to SURT, and synchronizing its label prediction with ASR token prediction through HAT-style blank factorization. In order to ensure consistency in relative speaker labels across different utterance groups in a recording, we propose"speaker prefixing"-- appending each chunk with high-confidence frames of speakers identified in previous chunks, to establish the relative order. We perform extensive ablation experiments on synthetic LibriSpeech mixtures to validate our design choices, and demonstrate the efficacy of our final model on the AMI corpus.
  </details>

- **Training Early-Exit Architectures for Automatic Speech Recognition: Fine-Tuning Pre-Trained Models or Training from Scratch**
   G. Wright, Umberto Cappellazzo, Salah Zaiem, Desh Raj, Lucas Ondel Yang, Daniele Falavigna, Mohamed Nabih Ali, A. Brutti
   2024 IEEE International Conference on Acoustics, Speech, and Signal Processing Workshops (ICASSPW)
   [open paper page](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10627008)
   <details>
     <summary> Abstract </summary>
     The ability to dynamically adjust the computational load of neural models during inference is crucial for on-device processing scenarios characterised by limited and time-varying computational resources. A promising solution is presented by early-exit architectures, in which additional exit branches are appended to intermediate layers of the encoder. In self-attention models for automatic speech recognition (ASR), early-exit architectures enable the development of dynamic models capable of adapting their size and architecture to varying levels of computational resources and ASR performance demands. Previous research on early-exiting ASR models has relied on pre-trained self-supervised models, fine-tuned with an early-exit loss. In this paper, we undertake an experimental comparison between fine-tuning pre-trained backbones and training models from scratch with the early-exiting objective. Experiments conducted on public datasets reveal that early-exit models trained from scratch not only preserve performance when using fewer encoder layers but also exhibit enhanced task accuracy compared to single-exit or pre-trained models. Furthermore, we explore an exit selection strategy grounded in posterior probabilities as an alternative to the conventional frame-based entropy approach. Results provide insights into the training dynamics of early-exit architectures for ASR models, particularly the efficacy of training strategies and exit selection methods.
  </details>

- **Bypass Temporal Classification: Weakly Supervised Automatic Speech Recognition with Imperfect Transcripts**
   Dongji Gao, Matthew Wiesner, Hainan Xu, Leibny Paola García, Daniel Povey, S. Khudanpur
   Interspeech 2023
   [open paper page](https://arxiv.org/pdf/2306.01031.pdf)
   <details>
     <summary> Abstract </summary>
     This paper presents a novel algorithm for building an automatic speech recognition (ASR) model with imperfect training data. Imperfectly transcribed speech is a prevalent issue in human-annotated speech corpora, which degrades the performance of ASR models. To address this problem, we propose Bypass Temporal Classification (BTC) as an expansion of the Connectionist Temporal Classification (CTC) criterion. BTC explicitly encodes the uncertainties associated with transcripts during training. This is accomplished by enhancing the flexibility of the training graph, which is implemented as a weighted finite-state transducer (WFST) composition. The proposed algorithm improves the robustness and accuracy of ASR systems, particularly when working with imprecisely transcribed speech corpora. Our implementation will be open-sourced.
  </details>

- **Learning From Flawed Data: Weakly Supervised Automatic Speech Recognition**
   Dongji Gao, Hainan Xu, Desh Raj, Leibny Paola Garcia Perera, Daniel Povey, S. Khudanpur
   Automatic Speech Recognition & Understanding 2023
   [open paper page](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10389684)
   <details>
     <summary> Abstract </summary>
     Training automatic speech recognition (ASR) systems requires large amounts of well-curated paired data. However, human annotators usually perform “non-verbatim” transcription, which can result in poorly trained models. In this paper, we propose Omni-temporal Classification (OTC), a novel training criterion that explicitly incorporates label uncertainties originating from such weak supervision. This allows the model to effectively learn speech-text alignments while accommodating errors present in the training transcripts. OTC extends the conventional CTC objective for imperfect transcripts by leveraging weighted finite state transducers. Through experiments conducted on the LibriSpeech and LibriVox datasets, we demonstrate that training ASR models with OTC avoids performance degradation even with transcripts containing up to 70% errors, a scenario where CTC models fail completely. Our implementation is available at https://github.com/k2-fsa/icefall.
  </details>


- **SURT 2.0: Advances in Transducer-Based Multi-Talker Speech Recognition**
   Desh Raj, Daniel Povey, S. Khudanpur
   IEEE/ACM Transactions on Audio Speech and Language Processing 2023
   [open paper page](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10262308)
   <details>
     <summary> Abstract </summary>
     The Streaming Unmixing and Recognition Transducer (SURT) model was proposed recently as an end-to-end approach for continuous, streaming, multi-talker speech recognition (ASR). Despite impressive results on multi-turn meetings, SURT has notable limitations: (i) it suffers from leakage and omission related errors; (ii) it is computationally expensive, due to which it has not seen adoption in academia; and (iii) it has only been evaluated on synthetic mixtures. In this work, we propose several modifications to the original SURT which are carefully designed to fix the above limitations. In particular, we (i) change the unmixing module to a mask estimator that uses dual-path modeling, (ii) use a streaming zipformer encoder and a stateless decoder for the transducer, (iii) perform mixture simulation using force-aligned subsegments, (iv) pre-train the transducer on single-speaker data, (v) use auxiliary objectives in the form of masking loss and encoder CTC loss, and (vi) perform domain adaptation for far-field recognition. We show that our modifications allow SURT 2.0 to outperform its predecessor in terms of multi-talker ASR results, while being efficient enough to train with academic resources. We conduct our evaluations on 3 publicly available meeting benchmarks — LibriCSS, AMI, and ICSI, where our best model achieves WERs of 16.9%, 44.6% and 32.2%, respectively, on far-field unsegmented recordings.
  </details>
- **Building Keyword Search System from End-To-End Asr Systems**
   Ruizhe Huang, Matthew Wiesner, Leibny Paola García-Perera, Daniel Povey, J. Trmal, S. Khudanpur
   IEEE International Conference on Acoustics, Speech, and Signal Processing 2023
   [open paper page](http://ieeexplore.ieee.org/stamp/stamp.jsp?tp=&arnumber=10097249)
   <details>
     <summary> Abstract </summary>
     Keyword search (KWS) systems are commonly built on top of existing automatic speech recognition (ASR) systems. However, end-to-end (E2E) ASR models are not naturally equipped with word-level timing information or confidence. Existing methods for re-purposing E2E ASR systems for KWS are largely heuristic or model-specific. In this paper, we describe a general KWS pipeline, applicable to any ASR model that generates N-best lists. We extract timing information using either external word-aligners, or time-preserving weighted finite-state transducer-based decoders. We show that our light-weight, ASR-agnostic approach for confidence estimation based on N-best lists outperforms other commonly used heuristics, such as using the decoder’s softmax probability, and even a more complicated dedicated confidence estimation model (CEM). Finally, we compare our performance to hybrid ASR models, extensively evaluating the impact of word-level timing, confidence, and recall on KWS performance. Our KWS pipeline is available online1, suitable for evaluating the aforementioned ASR components as downstream tasks.
     
  </details>
- **JHU IWSLT 2023 Dialect Speech Translation System Description**
   A. Hussein, Cihan Xiao, Neha Verma, Thomas Thebaud, Matthew Wiesner, S. Khudanpur
   International Workshop on Spoken Language Translation 2023
   [open paper page](https://api.semanticscholar.org/CorpusId:259376822)
   <details>
     <summary> Abstract </summary>
     This paper presents JHU’s submissions to the IWSLT 2023 dialectal and low-resource track of Tunisian Arabic to English speech translation. The Tunisian dialect lacks formal orthography and abundant training data, making it challenging to develop effective speech translation (ST) systems. To address these challenges, we explore the integration of large pre-trained machine translation (MT) models, such as mBART and NLLB-200 in both end-to-end (E2E) and cascaded speech translation (ST) systems. We also improve the performance of automatic speech recognition (ASR) through the use of pseudo-labeling data augmentation and channel matching on telephone data. Finally, we combine our E2E and cascaded ST systems with Minimum Bayes-Risk decoding. Our combined system achieves a BLEU score of 21.6 and 19.1 on test2 and test3, respectively.
  </details>
  
- **Defense against Adversarial Attacks on Hybrid Speech Recognition System using Adversarial Fine-tuning with Denoiser**
   Sonal Joshi, Saurabh Kataria, Yiwen Shao, Piotr Żelasko, J. Villalba, S. Khudanpur, N. Dehak
   Interspeech 2022
   [open paper page](https://doi.org/10.21437/interspeech.2022-10977)
   <details>
     <summary> Abstract </summary>
     Adversarial attacks are a threat to automatic speech recognition (ASR) systems, and it becomes imperative to propose defenses to protect them. In this paper, we perform experiments to show that K2 conformer hybrid ASR is strongly affected by white-box adversarial attacks. We propose three defenses–denoiser pre-processor, adversarially fine-tuning ASR model, and adversarially fine-tuning joint model of ASR and denoiser. Our evaluation shows denoiser pre-processor (trained on offline adversarial examples) fails to defend against adaptive white-box attacks. However, adversarially fine-tuning the denoiser using a tandem model of denoiser and ASR offers more robustness. We evaluate two variants of this defense–one updating parameters of both models and the second keeping ASR frozen. The joint model offers a mean absolute decrease of 19.3% ground truth (GT) WER with reference to baseline against fast gradient sign method (FGSM) attacks with different L∞ norms. The joint model with frozen ASR parameters gives the best defense against projected gradient descent (PGD) with 7 iterations, yielding a mean absolute increase of 22.3% GT WER with reference to baseline; and against PGD with 500 iterations, yielding a mean absolute decrease of 45.08% GT WER and an increase of 68.05% adversarial target WER.
  </details>

- **GPU-accelerated Guided Source Separation for Meeting Transcription**
   Desh Raj, Daniel Povey, S. Khudanpur
   Interspeech 2022
   [open paper page](https://arxiv.org/pdf/2212.05271.pdf)
   <details>
     <summary> Abstract </summary>
     Guided source separation (GSS) is a type of target-speaker extraction method that relies on pre-computed speaker activities and blind source separation to perform front-end enhancement of overlapped speech signals. It was first proposed during the CHiME-5 challenge and provided significant improvements over the delay-and-sum beamforming baseline. Despite its strengths, however, the method has seen limited adoption for meeting transcription benchmarks primarily due to its high computation time. In this paper, we describe our improved implementation of GSS that leverages the power of modern GPU-based pipelines, including batched processing of frequencies and segments, to provide 300x speed-up over CPU-based inference. The improved inference time allows us to perform detailed ablation studies over several parameters of the GSS algorithm -- such as context duration, number of channels, and noise class, to name a few. We provide end-to-end reproducible pipelines for speaker-attributed transcription of popular meeting benchmarks: LibriCSS, AMI, and AliMeeting. Our code and recipes are publicly available: https://github.com/desh2608/gss.
  </details>

- **Chunking Defense for Adversarial Attacks on ASR**
  Yiwen Shao, J. Villalba, S. Joshi, S. Kataria, S. Khudanpur, N. Dehak
  Interspeech 2022
  [open paper page](https://www.isca-archive.org/interspeech_2022/shao22c_interspeech.pdf)
  <details>
    <summary> Abstract </summary>
    While deep learning has lead to dramatic improvements in automatic speech recognition (ASR) systems in the past few years, it has also made them vulnerable to adversarial attacks. These attacks may be designed to either make ASR fail in producing the correct transcription or worse, output an adversary-chosen sentence. In this work, we propose a defense based on independently processing random or fixed size chunks of the speech input in the hope of "containing” the cumulative effect of the adversarial perturbations. This approach does not require any additional training of the ASR system, or any defensive preprocessing of the input. It can be easily applied to any ASR systems with little loss in performance under benign conditions, while improving adversarial robustness. We perform experiments on the Librispeech data set with different adversarial attack budgets, and show that the proposed defense achieves consistent improvement on two different ASR systems/models.
  </details>
