# 02_Data

대용량 입력 데이터와 모델 가중치는 GitHub에 포함하지 않습니다. Colab에서는 공유 폴더 `0_ASAC_11기_DL_4조`를 Google Drive의 **내 드라이브에 바로가기**로 추가한 뒤 다음 경로를 사용합니다.

폴더를 다른 위치나 이름으로 저장했다면 각 노트북의 설정 셀에서 `DATA_ROOT`를 실제 경로로 수정하면 됩니다.

```text
/content/drive/MyDrive/0_ASAC_11기_DL_4조/02_Data
```

## 폴더 구조

```text
raw_room/
  room01/ ... room06/      방 이미지
  room01_empty/
  room06_empty/
raw_video/
  room.mov                 최종 시연 원본 영상
  sk304_2.mov              304호 시연 원본 영상
raw_furniture/             가구 원본 이미지
furniture_glb/             배치용 가구 GLB
pointmap/                  생성된 포인트클라우드
final_glb/                 최종 결과물
room##_seg_labels.npz      수동 세그멘테이션 마스크
room##_seg_labels.json     수동 세그멘테이션 메타데이터
yolo11s_1074_832_final_20260703.pt
yolo11s_train.pt
```

## 개인정보 및 공개 범위

실제 거주 공간을 촬영한 영상과 이미지는 구조, 위치 단서, 개인 물품을 포함할 수 있습니다. 원본 제공자의 명시적 동의가 없는 `raw_room`과 `raw_video`는 공개 저장소에 업로드하지 않습니다. 저장소에는 비식별 샘플 또는 결과 이미지와 데이터 구조만 포함합니다.
