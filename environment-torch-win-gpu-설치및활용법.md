- 윈도우 용 Miniforge 설치 후 Miniforge Prompt 활용하여 환경 업데이트 및 설치
- bash 환경을 environment.base.yml 이용 업데이트
- 이후 아래 명령어를 통해 Pytorch GPU 환경 설치

```
mamba env create -f C:\Users\gslee\Documents\GitHub\code-workout-ml\environment-torch-win-gpu.yml -p C:\Users\gslee\miniforge3\envs\tw-gpu
```

- 권장 워크플로우 (Miniforge 사용 시):

    1) 환경 생성 및 패키지 설치 (빠른 속도 필요 시):

    ```
    mamba env create -f environment.yml
    mamba install <패키지명>
    ```

    2) 환경 활성화 및 비활성화 (안정성 필요 시):

    ```
    conda activate <환경이름>
    conda deactivate
    ```

    3) 셸 초기화 (필요한 경우에만):

    ```
    conda init <셸이름>  # (mamba init은 사용 금지)
    ```

- tw-gpu 환경 삭제할 때:

```
mamba env remove -p C:\Users\gslee\miniforge3\envs\tw-gpu
```
