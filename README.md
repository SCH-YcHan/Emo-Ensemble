# Emo-Ensemble
[Competition] [제 2회 ETRI 휴먼이해 인공지능 논문경진대회](https://aifactory.space/competition/qna/2234/1019)  
[Paper] Emo-Ensemble: An Ensemble-based Multimodal Emotion Recognition using wav2vec2 and KoBERT

## 1. Original Data Source
[KEMDy20] [한국어 멀티모달 감정데이터셋 2020](https://nanum.etri.re.kr/share/kjnoh/KEMDy20?lang=ko_KR)  
<img src="https://user-images.githubusercontent.com/113504815/232485081-a0b3e3fe-78b2-42be-ac54-185945990cd7.png" width="600" height="90">  

[AI Hub] [감정 분류를 위한 대화 음성 데이터셋](https://aihub.or.kr/aihubdata/data/view.do?currMenu=115&topMenu=100)  
<img src="https://user-images.githubusercontent.com/113504815/232484969-550c167a-f9a6-438e-b08f-ff75a84d7efa.png" width="600" height="150">

## 2. Environment
### Local
```
OS: Windows 10 Pro
CPU: Intel(R) Core(TM) i9-10900X 
GPU: NVIDIA GeForce RTX 2080 Ti
CUDA version: 11.7
CuDNN version: 8.4.0
Workstation: Anaconda3
```
```
# Anaconda env setting
conda create -n ETRI python=3.9
activate ETRI
conda install pytorch torchvision torchaudio-cuda=11.7 -c pytorch -c nvidia
conda install jupyter notebook
```
```
# Clone Emo-Ensemble github
git clone https://github.com/SCH-YcHan/Emo-Ensemble.git
```
```
# Requires packages install
pip install -r requirements.txt
```
### Colab
```
Colab version: Colab Pro
```

## 3. Directory
### Local
```
ETRI (폴더를 새로 생성하여 폴더 내부에서 git clone을 수행)
├── Emo-Ensemble (git clone)
│   ├── code
│   │   ├── 1. Annotation preprocessing & Data split (Local).ipynb
│   │   ├── 2. Confirm class distribution (Local).ipynb
│   │   ├── 3. Text preprocessing (Local).ipynb
│   │   ├── 4. Save SER dataset (Local).ipynb
│   │   ├── 5. Emotion Recognition with KoBERT (Colab).ipynb ─────────────┐ Colab으로 
│   │   ├── 6. Emotion Recognition with wav2vec2 (Colab).ipynb ───────────┘ 옮겨주어야 함
│   │   ├── 7. Emotion Recognition with wav2vec2 (Local).ipynb
│   │   ├── 8. Ensemble prediction (Local).ipynb
│   │   └── try (Emo-Ensemble 모델 구현에 사용되지 않는 코드들)
│   ├── Class_distribution_add.png (KEMDy20 + AI Hub class distribution)
│   ├── Class_distribution_origin.png (KEMDy20 class distribution)
│   ├── Readme.md
│   └── requirements.txt
├── KEMDy20_v1_1 (KEMDy20 Dataset)
│   ├── annotation
│   │   ├── Sess01_eval.csv
│   │   ├── ...
│   │   └── Sess40_eval.csv
│   ├── EDA
│   ├── IBI
│   ├── TEMP
│   ├── wav
│   │   ├── Session03
│   │   ├── ...
│   │   └── Session40
└── AI_Hub (AI Hub Dataset)
    ├── annotation
    │   └── 5차년도_2차.csv
    └── wav
        ├── 5f3c9ed98a3c1005aa97c4bd.wav
        ├── ...
        └── 5fbe364744697678c497c07f.wav
```
### Colab
```
├── ETRI
    │   ├── file11.ext
    │   └── file12.ext
    ├── dir2
    │   ├── file21.ext
    │   ├── file22.ext
    │   └── file23.ext
    ├── dir3
    ├── file_in_root.ext
    └── README.md
```

## Pretrained Model info

### wav2vec2

### KoBERT

## 4. Benchmark Model info
[MMM: Multi-modal Emotion Recognition in conversation with MLP Mixer](https://github.com/ISDS-Human-Understanding/HumanUnderstandingOpen)

## 5. Emo-Ensemble hyper-parameters

### wav2vec2

### KoBERT

## 6. Model Architecture

## 7. Experiment results

### Fig 1. Class distribution (KEMDy20)
<img src="Class_distribution_origin.png">

### Fig 2. Class distribution (KEMDy20 + AI Hub)
<img src="Class_distribution_add.png">
