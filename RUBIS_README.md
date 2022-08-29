## RUBIS_README
RUBIS 연구실 UROP를 위한 KR-BERT repository입니다.
학습이나 pretrained weight을 위한 설명은 `README.md`를 참고해주세요.

### Changelog
- tensorflow 2.X 버전과의 호환을 위해 import 및 라인 몇줄이 수정되었습니다.
- 이해를 돕기위한 notebook 파일을 추가했습니다. (`krbert_pytorch/KR_BERT_inference.ipynb`)
- `.gitignore` 파일을 추가했습니다.
- 설치를 위한 `requirements.txt`를 추가했습니다.
    - 다음과 같은 커맨드로 필요 패키지를 설치할 수 있으나, 개인 사용환경(OS, python 버전)에 따라 변경이 필요할 수 있으니 확인 부탁드립니다.
    ```
    pip3 install -r requirements.txt
    ```

### Training
```
python3 train.py --subchar False --tokenizer ranked
```

### Inference
- 학습을 완료하면 `checkpoints/best_snu_char16424_rannked.tar`이 생성되고, 이 weight을 가지고 notebook 파일을 실행할 수 있습니다.
