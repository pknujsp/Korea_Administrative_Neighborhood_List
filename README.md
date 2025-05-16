## 대한민국 행정동 목록(SQLite, CSV, JSON)

행정동 코드와 좌표(위경도)를 포함하는 행정동 목록입니다.

웹 상에서 코드와 좌표가 같이 포함된 목록을 찾을 수 없어 만들게 되었습니다.

## 제작 방법

[기상청 날씨누리](https://www.weather.go.kr/w/index.do) 페이지 내에서 제공하는 **읍면동** 목록을 파싱

## 파일별 형식

### CSV, DB

| district_code(행정동 코드) | province_code(시,도 코드) | city_code(시,군,구 코드) | province       | city   | district | latitude | longitude |
| -------------------------- | ------------------------- | ------------------------ | -------------- | ------ | -------- | -------- | --------- |
| 5115061500                 | 5100000000                | 5115000000               | 강원특별자치도 | 강릉시 | 강남동   | 37.74421 | 128.90561 |
| 5115034000                 | 5100000000                | 5115000000               | 강원특별자치도 | 강릉시 | 강동면   | 37.7254  | 128.95651 |
| 5115066500                 | 5100000000                | 5115000000               | 강원특별자치도 | 강릉시 | 경포동   | 37.78101 | 128.88289 |

### JSON

```json
[
    {
        "name": "강원특별자치도",
        "code": "5100000000",
        "sub": [
            {
                "code": "5115000000",
                "name": "강릉시",
                "shortName": "강릉시",
                "x": "92",
                "y": "131",
                "lat": "37.749138",
                "lon": "128.8785",
                "level": "2",
                "nameEn": "Gangneung-si",
                "shortNameEn": "Gangneung-si",
                "sub": [
                    {
                        "code": "5115061500",
                        "name": "강남동",
                        "shortName": "강남동",
                        "x": "93",
                        "y": "131",
                        "lat": "37.74421",
                        "lon": "128.90561",
                        "level": "3",
                        "nameEn": "Gangnam-dong",
                        "shortNameEn": "Gangnam-dong"
                    },
                    {
                        "code": "5115034000",
                        "name": "강동면",
                        "shortName": "강동면",
                        "x": "94",
                        "y": "131",
                        "lat": "37.7254",
                        "lon": "128.95651",
                        "level": "3",
                        "nameEn": "Gangdong-myeon",
                        "shortNameEn": "Gangdong-myeon"
                    },
                    ...
    },
    {
        "name": "경기도",
        "code": "4100000000",
        "sub": [
            {
                "code": "4182000000",
                "name": "가평군",
                "shortName": "가평군",
                ...
```

## 업데이트

- **[2024.01.07](https://github.com/pknujsp/Korea_Administrative_Neighborhood_List/releases/tag/2024-01-07)**: 첫번째 버전
- **[2025.05.16](https://github.com/pknujsp/Korea_Administrative_Neighborhood_List/releases/tag/2025-05-16)**: 두번째 버전

