<div align="center">
  <strong>English</strong> | <a href="./README.zh-CN.md">简体中文</a>
</div>
<br />

# JAV Metadata API

![API Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

A simple, high-performance HTTP API for retrieving structured metadata for JAV (Japanese Adult Video) movies. This service allows you to query movie details using a designation ID and returns formatted **JSON** data.

## 🔗 Base URL

All requests are made to:
`https://api.thejavdb.net/v1`

## 📚 Documentation

For interactive documentation and testing, visit our Swagger UI:

👉 **[View Full API Documentation](https://api.thejavdb.net/v1/doc)**

## 🔍 Usage

Currently, the API supports a search endpoint to retrieve metadata by movie ID (designation).

### Endpoint

`GET /movies`

### Parameters

| Parameter | Type   | Required | Description                                      |
| :-------- | :----- | :------- | :----------------------------------------------- |
| `q`       | string | **Yes** | The movie designation/ID (e.g., `SSIS-001`) |

### Example Request (cURL)

```bash
curl -X GET "https://api.thejavdb.net/v1/movies?q=SSIS-001" \
     -H "Accept: application/json"
```

### Sample JSON Response
```json
{
  "universal_id": "SSIS-001",
  "title": "一ヶ月間の禁欲の果てに彼女のルームメイト2人と浮気SEXだけに没頭した彼女不在の3日間。 葵つかさ 乙白さやか",
  "description": "S1スリム美女優の豪華共演エモドラマ作！僕の彼女は友人2人とルームシェアをしている。僕もたまにその家に遊びにいくのだが年上でクールなルームメイト‘つかさ’に恋してしまい告白。彼女と一か月間エッチしなければイイ事してあげると言われ僕は禁欲生活の末にセックス。彼女は不在中だったがそれをもう一人の友人‘さやか’に見られ逆告白、なりゆきでエッチする。こじれた淫らな彼女不在の3日間のハメまくりNTR生活。",
  "fullcover_url": "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001pl.jpg",
  "frontcover_url": "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001ps.jpg",
  "sample_movie_url": "https://cc3001.dmm.co.jp/pv/MAwkRhEUIKm3Bpw46XbYlJ0632Em9cInMYE3mfoYX5LCf2mT97-mU28dgV_c5y/ssis00001_mhb_w.mp4",
  "release_date": "2021-02-18",
  "duration": 147,
  "source_url": "https://video.dmm.co.jp/av/content/?id=ssis00001",
  "maker": "エスワン ナンバーワンスタイル",
  "label": "S1 NO.1 STYLE",
  "series": null,
  "actresses": [
    "葵つかさ",
    "乙白さやか"
  ],
  "directors": [
    "苺原"
  ],
  "genres": [
    "ハイビジョン",
    "美少女",
    "寝取り・寝取られ・NTR",
    "美乳",
    "3P・4P",
    "独占配信",
    "ドラマ",
    "ギリモザ"
  ],
  "samples": [
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-1.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-2.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-3.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-4.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-5.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-6.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-7.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-8.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-9.jpg",
    "https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-10.jpg"
  ]
}
```

## 📡 Data Sources

Currently, this API provides metadata for a **limited subset** of videos from **[https://video.dmm.co.jp](https://video.dmm.co.jp)**.

* **Future Plans:** We may add support for other websites (e.g. [https://www.mgstage.com](https://www.mgstage.com)) in upcoming versions.

## ⚠️ Disclaimer
Content Warning: This API provides metadata regarding adult content. By using this API, you confirm that you are of legal age in your jurisdiction to view such content.

Copyright: This API provides metadata indexing only. It does not host, distribute, or provide links to download video files. All metadata rights and images belong to their respective copyright holders.

## 📄 License
This project is open-source and licensed under the MIT License.
