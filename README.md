1. KoBERT_keras_2
2. KoBERT_keras_2_del_neu
3. KoBERT_keras_2_netral_undersampling
4. KoBERT_4_labels
5. emotion_base_recomnnedation

# 0. Introdunction

- colab 환경에서 진행되었습니다
- TPU, HuggingFace의 Transformers, SKTBrain의 KoBERT tokenizer & model을 활용해 진행하였고, random seed는 1234로 고정했습니다

<br>

# 0.1 Source Data

- 7종 감정 라벨링<br>
  분노, 놀람, 행복, 슬픔, 혐오, 공포, 중립<br>

- [한국어 감정 정보가 포함된 단발성 대화 데이터](https://aihub.or.kr/opendata/keti-data/recognition-laguage/KETI-02-009)

- [한국어 감정 정보가 포함된 연속적 대화 데이터셋](https://aihub.or.kr/opendata/keti-data/recognition-laguage/KETI-02-010)

- [감정 분류를 위한 대화 음성 데이터셋](https://aihub.or.kr/opendata/keti-data/recognition-laguage/KETI-02-002)

<br>

# 1. Pre-Process Data

## 1) re-labeling
- 가사 감정분석의 목적에 맞게 '중립' 라벨 제거, '분노'와 '혐오' 그리고 '놀람'과 '공포' 라벨을 합쳤습니다

- Class Distribution
  - 분노혐오    20526
  - 놀람공포    19471
  - 행복       11615
  - 슬픔       10087

<img width=40% height=40% src="https://user-images.githubusercontent.com/78069770/171363414-a8871cfb-31a0-4bee-b3f7-9e323c854fe5.png">

- Digitizing Label<br>
  - 분노+혐오 : 0 
  - 놀람+공포 : 1
  -     슬픔 : 2
  -     행복 : 3


<br>

# 2. Modeling

<br>

# 3. Train

<br>

# 4. Test

<br>

# 5. Save Model


<br>

# 6. Load Saved Model

- pickle 파일 load, input 데이터로 전처리, 분석의 코드입니다
