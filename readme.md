# pypi 등록 방법
### <br/><br/><br/>

## 1. directory 준비
### 만들어야 할 파일
1. setup.py
2. \[package_dir\]/스크립트들
3. \[package_dir\]/__init__.py
4. readme.md
5. LICENSE.txt (option)
### ![image](https://user-images.githubusercontent.com/62974484/208827509-e4074274-254f-4161-ad35-b2e46fb02231.png)
### <br/><br/><br/>

## 2. 파일 준비
### 1) setup.py
- name : 패키지 명
- version : 버전
  #### 주의할 사항 : 패키지 명 + 버전은 패키지를 삭제하였더라도 무조건 겹치면 안 된다. 안 그러면 에러 난다.
- long_description, long_description_content_type : 똑같이 채워 넣는다.
- url : 안 써도 된다.
- classifiers : 패키지를 만들고 나서 왼쪽 사이드메뉴에 명시된다.
  #### ![image](https://user-images.githubusercontent.com/62974484/208828129-290f09e7-b75a-495f-82e6-1550ed153efd.png)
```
import setuptools

with open("readme.md", "r") as fh:
    long_description = fh.read()

setuptools.setup(
    name="shinejh0528_bioinfo_parser", # Replace with your own username
    version="0.0.4",
    author="Jonghwan Shin",
    author_email="shinejh0528@gmail.com",
    description="Bioinfomatics parser",
    long_description=long_description,
    long_description_content_type="text/markdown",
    url="https://github.com/Shin-jongwhan/python_pypi/tree/main/bioinfo_parser",
    packages=setuptools.find_packages(),
    classifiers=[
        "Programming Language :: Python :: 3",
        "License :: OSI Approved :: MIT License",
        "Operating System :: OS Independent",
    ],
    python_requires='>=3.6',
)
```


## 3. import 하고 사용하기
### 설치
#### ![image](https://user-images.githubusercontent.com/62974484/208827295-b6082ee3-87c2-4dea-b1d6-4cfef8724fda.png)
### 설치 확인
#### ![image](https://user-images.githubusercontent.com/62974484/208827222-2320c552-3065-412f-a5cd-ca2b29bbebcf.png)
#### ![image](https://user-images.githubusercontent.com/62974484/208827327-2330e867-3998-48f3-881a-c775137fc45e.png)
### <br/><br/><br/>
