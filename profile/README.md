# 개인 맞춤형 아파트 실거래가 조회 서비스

- 프로젝트명: WHERE IS MY HOME
- 프로젝트 주제: 개인 맞춤형 아파트 실거래가 조회 서비스
- 개발 기간: 2022.11.16.~2022.11.25.(10일)
- 사용 기술 스택: Spring, MySQL, Vue.js, Vite, JavaScript, Git

## 1. 프로젝트 설명

WHERE IS MY HOME은 개인 맞춤형 아파트 실거래가 조회 서비스로, 단순한 과거 아파트 실거래가 조회 기능 외에도 사용자의 관심사에 특화된 맞춤 정보 및 자세한 리뷰 시스템을 제공합니다.

최근 공급자 주도의 '대량 소비'가 저물고, 소비자 주도의 '개인 맞춤'이 트렌드로 떠오르고 있습니다 [[출처](https://blog.logi-spot.com/%EB%AC%BC%EB%A5%98-%EC%97%B0%EA%B5%AC%EC%86%8C-%E2%91%A6-mz-%EC%82%AC%EB%A1%9C%EC%9E%A1%EC%9C%BC%EB%A0%A4%EB%A9%B4-%EA%B0%9C%EC%9D%B8%EB%A7%9E%EC%B6%A4%ED%95%98%EB%9D%BC/)]. 하지만 기존의 실거래가 조회 서비스는 과거 기록 조회 기능에 충실해 소비자 맞춤 서비스가 부족합니다.

따라서 WHERE IS MY HOME은 급변하고 있는 가족 형태, 다양해진 관심사에 맞춰 개인화된 아파트 검색 서비스를 제공하며, 사전 지식 없이 누구나 한눈에 원하는 정보를 파악할 수 있도록 데이터 시각화 서비스 및 상세한 리뷰 시스템 또한 구현했습니다.

## 2. 주요 기능

|                                         회원가입                                          |                                       로그인                                        |
| :---------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------: |
| ![register](https://github.com/final0809/frontend/raw/main/resources/images/register.png) | ![login](https://github.com/final0809/frontend/raw/main/resources/images/login.JPG) |
|               회원 가입 시, 입력 정보에 대한<br/>유효성 체크를 수행합니다.                |                                                                                     |

|                                          동별 아파트 검색                                           |                                          주변 상권 정보                                          |
| :-------------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------------------: |
| ![dong_search](https://github.com/final0809/frontend/raw/main/resources/images/search-apt-list.JPG) | ![nearby](https://github.com/final0809/frontend/raw/main/resources/images/search-apt-nearby.png) |
|             원하는 동을 선택해 검색하면<br/>해당 동의 아파트 정보를 지도에 표시합니다.              |                      카카오맵 API를 활용해<br/>주변 상권 정보를 표시합니다.                      |

|                                                                        아파트 기본 정보 화면                                                                         |                                               아파트 실거래가 정보 화면                                               |
| :------------------------------------------------------------------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------------------: |
|                            ![apartment_info](https://github.com/final0809/frontend/raw/main/resources/images/search-apt-detail-basic.JPG)                            | ![apartment_deal_info](https://github.com/final0809/frontend/raw/main/resources/images/search-apt-detail-records.gif) |
| 리스트 또는 지도에서 아파트를 클릭하면<br/>해당 아파트의 정보를 사이드 바에 표시합니다.<br/>로그인한 경우, 별 모양 버튼을 눌러<br/>관심 아파트로 추가할 수 있습니다. |    아파트의 최근 실거래가 및 평형별 최근 3년간 월별 평균 실거래가(상한가, 하한가, 평균가)를 차트로 볼 수 있습니다.    |

|                                       아파트 맞춤 정보 화면(로그인 X)                                        |                                      아파트 맞춤 정보 화면(로그인 O)                                      |
| :----------------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------------------------: |
| ![](https://github.com/final0809/frontend/raw/main/resources/images/search-apt-detail-interest-no-login.JPG) | ![](https://github.com/final0809/frontend/raw/main/resources/images/search-apt-detail-interest-login.JPG) |
|                    로그인하지 않고 맞춤 정보에 접근했을 때는<br/> 회원 가입을 유도합니다.                    |             로그인한 경우, 해당 사용자가 기존에 설정한<br/> 관심사에 맞는 정보를 표시합니다.              |

|                                             관심 지역 화면                                             |                                    관심 아파트 화면                                     |
| :----------------------------------------------------------------------------------------------------: | :-------------------------------------------------------------------------------------: |
|        ![](https://github.com/final0809/frontend/raw/main/resources/images/mypage-fav-loc.gif)         | ![](https://github.com/final0809/frontend/raw/main/resources/images/mypage-fav-apt.png) |
| 사용자가 등록한 관심 지역 목록 및 해당 지역의 뉴스, 매매 가격 지수 추이를 한 곳에 모아 볼 수 있습니다. |        사용자가 등록한 관심 아파트 목록 및 위치를 지도로 볼 수 있도록 했습니다.         |

|                                     리뷰 관리 화면                                      |                                    1:1 문의 화면                                    |
| :-------------------------------------------------------------------------------------: | :---------------------------------------------------------------------------------: |
| ![](https://github.com/final0809/frontend/raw/main/resources/images/mypage-reviews.png) | ![](https://github.com/final0809/frontend/raw/main/resources/images/mypage-qna.png) |
|                 사용자가 작성한 리뷰를<br/>관리할 수 있는 페이지입니다.                 |                사용자가 문의 사항을<br/> 남길 수 있는 페이지입니다.                 |
|                                                                                         |

|                                회원 정보 관리 화면 (인증 전)                                 |                            회원 정보 관리 화면 (인증 후)                             |
| :------------------------------------------------------------------------------------------: | :----------------------------------------------------------------------------------: |
| ![](https://github.com/final0809/frontend/raw/main/resources/images/mypage-info-checkpw.png) | ![](https://github.com/final0809/frontend/raw/main/resources/images/mypage-info.png) |
|                  회원 정보를 보기 전<br/>한 번 더 비밀번호 인증을 거칩니다.                  |                사용자가 개인 정보를<br/>관리할 수 있는 페이지입니다.                 |

|                              공지사항 화면 (일반 사용자)                               |                                공지사항 화면 (관리자)                                 |
| :------------------------------------------------------------------------------------: | :-----------------------------------------------------------------------------------: |
|  ![](https://github.com/final0809/frontend/raw/main/resources/images/notice-list.JPG)  | ![](https://github.com/final0809/frontend/raw/main/resources/images/notice-admin.JPG) |
| ![](https://github.com/final0809/frontend/raw/main/resources/images/notice-detail.JPG) | ![](https://github.com/final0809/frontend/raw/main/resources/images/notice-write.JPG) |
|         공지사항 목록 조회 및 상세 게시물 조회를<br/>할 수 있는 페이지입니다.          |  관리자 계정으로 로그인되어 있는 경우에만<br/>공지사항 작성/수정/삭제가 가능합니다.   |
