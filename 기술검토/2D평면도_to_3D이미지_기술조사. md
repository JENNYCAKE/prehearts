# 2D 평면도를 3D로 변환하는 AI 기술 검토

## 개요

복합 문화공간이나 영화관, 마트 등에서는 층별로 평면안내도 형태의 지도를 3D 또는 2.5D 지도로 구현하는 사례가 많습니다.  
우리가 만들고자 하는 툴에서도 2D 평면도를 3D로 변환하는 AI 또는 툴이 가능한지 조사하였습니다.

---

## 반자동

반자동 툴의 경우는 아래와 같은 도구들이 있습니다.

| 도구                | 자동 변환             | 커스터마이징     | 난이도 | 라이선스   |
|---------------------|------------------------|------------------|--------|------------|
| **Planner 5D**      | ✅ AI 인식              | ✅ 고급 옵션      | 낮음   | Freemium   |
| **Coohom**          | ❌ (직접 제작 중심)     | ✅                | 낮음   | Freemium   |
| **SketchUp**        | ❌ (직접 모델링)        | ✅ 고급 기능      | 중간   | 유료       |
| **Revit**           | ✅ CAD 기반 변환        | ✅ 전문가용       | 높음   | 유료       |
| **RoomSketcher**    | ❌                    | ✅                | 낮음   | Freemium   |
| **Sweet Home 3D**   | ❌ (수동)              | ✅                | 낮음   | 무료       |

---

### **Planner 5D**

- 실제로 사용 가능한 것으로 보이는 2D 도면 (PDF, PNG, JPG 등)을 3D로 변환해주는 유일한 툴.
- 다만, 유료 플랜을 구독해야 하며 프로그래밍적으로 활용하기 어려움. 사용자가 직접 이미지를 업로드해야 함.
- 링크: [Planner 5D](https://planner5d.com/ai)

---

### **Revit**

- CAD 기반 2D 도면을 3D로 변환하는 기능이 있음.
- 자동화보다는 전문가가 수동으로 작업하는 형태. 완전 자동화된 워크플로우 구성은 어려움.

---

### **Blender + Add-ons**

- Blender와 여러 애드온(Archimesh, Archipack 등)을 활용하면 사람이 2D 평면도를 기반으로 빠르게 3D 모델링 가능.
- 관련 설명은 [블렌더 기반 반자동화 툴 설명](#블렌더-기반-반자동화-툴)

---

### **그 외 툴**

- 대부분의 툴은 사람이 직접 웹 플랫폼에서 2D 평면도를 그려야 3D 변환이 가능.
- 자동화보다는 반자동 또는 수동 방식이 많음.

---

## 블렌더 기반 반자동화 툴

### **Archimesh / Archipack 애드온**

- Blender에 기본 또는 추가 설치 가능한 애드온.
- 벽, 문, 창문 등의 요소를 쉽게 생성 가능.
- 직관적인 UI와 건축 요소 프리셋 제공.

🔗 [Blender Architecture Addon Tutorial – Interior Design Floor Plan to 3D](https://www.youtube.com/watch?v=sF-iTbQYd0E)

---

### **HomeBuilder 애드온**

- 2D 평면도 이미지를 불러와 스케일 설정 후 3D 모델 생성.
- 이미지 기반의 빠른 모델링과 친숙한 UI 제공.

🔗 [The EASIEST Way to Create Floor Plans FROM IMAGES in Blender!](https://www.youtube.com/watch?v=sF-iTbQYd0E)

---

### **BlenderBIM 애드온**

- IFC 형식의 BIM 데이터를 지원하는 애드온.
- 2D 도면을 기반으로 건축 요소를 생성하고 3D 모델로 확장 가능.
- 정밀한 건축 모델링 가능.

🔗 [BlenderBIM - Floor plan - in 20mins (YouTube)](https://www.youtube.com/watch?v=xlmbZHIaHJw)

---

### **Tripo AI 튜토리얼**

- 2D 도면을 DXF 형식으로 내보낸 뒤 Blender에 불러오기.
- Archimesh 및 Archipack 애드온으로 3D 모델링 가능.

🔗 [Converting 2D Drawings to 3D Model in Blender - Tripo AI](https://www.youtube.com/watch?v=xlmbZHIaHJw)

---

## 자동

| 도구                | 자동 변환                 | 커스터마이징     | 난이도 | 라이선스   |
|---------------------|----------------------------|------------------|--------|------------|
| **Blender + Add-ons** | ✅ (개발자 셋업 필요)      | ✅                | 높음   | 오픈소스   |

---

### **FloorplanToBlender3D (오픈소스 프로젝트)**

- 2D 평면도 이미지를 분석해 자동으로 3D 모델을 생성.
- Python 기반으로 Docker에서 실행 가능.
- Swagger API를 통해 서버 형태로도 운영 가능.
- Jupyter Notebook 튜토리얼 제공.

🔗 [GitHub - FloorplanToBlender3D](https://github.com/grebtsew/FloorplanToBlender3d)

> *이 프로젝트는 기술 검증을 통해 추가 분석이 필요함.*
