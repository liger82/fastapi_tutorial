# fastapi_tutorial

## 소개

- FastAPI는 현대적이고, 빠르며(고성능), 파이썬 표준 타입 힌트에 기초한 Python3.6+의 API를 빌드하기 위한 웹 프레임워크입니다.
- https://fastapi.tiangolo.com/ko/ 
- 장점
    - 빠름: (Starlette과 Pydantic 덕분에) NodeJS 및 Go와 대등할 정도로 매우 높은 성능.(말은 그렇게 하는데 실제로는 fastapi가 더 느리다.) 사용 가능한 가장 빠른 파이썬 프레임워크 중 하나.
    - 빠른 코드 작성: 약 200%에서 300%까지 기능 개발 속도 증가. 
    - 적은 버그: 사람(개발자)에 의한 에러 약 40% 감소.
    - 직관적: 훌륭한 편집기 지원. 모든 곳에서 자동완성. 적은 디버깅 시간.
    - 쉬움: 쉽게 사용하고 배우도록 설계. 적은 문서 읽기 시간.
    - 짧음: 코드 중복 최소화. 각 매개변수 선언의 여러 기능. 적은 버그.
    - 견고함: 준비된 프로덕션 용 코드를 얻으세요. 자동 대화형 문서와 함께.
    - 표준 기반: API에 대한 (완전히 호환되는) 개방형 표준 기반: OpenAPI (이전에 Swagger로 알려졌던) 및 JSON 스키마
- 단점
    - 아직 정식 1.0 버전이 출시된 것이 아니다.

## 설치

```
$ pip install fastapi
# mac에서는 큰따옴표 붙이고 ubuntu에서는 생략
$ pip install "uvicorn[standard]"
```

## 실행

* main.py 파일이 있는 위치에서
    - port는 일부러 9000으로 지정(default:8000)  
    - --reload 코드 변경시 자동 reload됨
```
uvicorn main:app --reload --port 9000
```

* http://localhost:9000/docs : 자동 설계된 대화형 API 문서
* http://localhost:9000/redoc : 대안 API 문서