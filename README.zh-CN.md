<div align="center">
  <a href="./README.md">English</a> | <strong>简体中文</strong>
</div>
<br />

# JAV Metadata API

![API Status](https://img.shields.io/badge/status-active-success.svg)
![License](https://img.shields.io/badge/license-MIT-blue.svg)

这是一个简单、高性能的 HTTP API，用于获取 JAV（日本成人视频）电影的结构化元数据。该服务允许用户通过番号（Designation ID）查询详细信息，并返回格式化的 **JSON** 数据。

## 🔗 基础 URL (Base URL)

所有请求均应发送至：
`https://api.thejavdb.net/v1`

## 📚 文档

如需查看交互式文档和进行接口测试，请访问我们的 Swagger UI：

👉 **[查看完整 API 文档](https://api.thejavdb.net/v1/doc)**

## 🔍 使用方法

目前，API 支持通过电影番号（ID）进行搜索以获取元数据。

### 端点 (Endpoint)

`GET /movies`

### 参数

| 参数 | 类型   | 必填 | 描述                                      |
| :-------- | :----- | :------- | :----------------------------------------------- |
| `q`       | string | **是** | 电影番号 (例如 `SSIS-001`) |

### 请求示例 (cURL)

```bash
curl -X GET "[https://api.thejavdb.net/v1/movies?q=SSIS-001](https://api.thejavdb.net/v1/movies?q=SSIS-001)" \
     -H "Accept: application/json"
```

### JSON 响应示例
```json
{
  "universal_id": "SSIS-001",
  "title": "一ヶ月間の禁欲の果てに彼女のルームメイト2人と浮気SEXだけに没頭した彼女不在の3日間。 葵つかさ 乙白さやか",
  "description": "S1スリム美女優の豪華共演エモドラマ作！僕の彼女は友人2人とルームシェアをしている。僕もたまにその家に遊びにいくのだが年上でクールなルームメイト‘つかさ’に恋してしまい告白。彼女と一か月間エッチしなければイイ事してあげると言われ僕は禁欲生活の末にセックス。彼女は不在中だったがそれをもう一人の友人‘さやか’に見られ逆告白、なりゆきでエッチする。こじれた淫らな彼女不在の3日間のハメまくりNTR生活。",
  "fullcover_url": "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001pl.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001pl.jpg)",
  "frontcover_url": "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001ps.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001ps.jpg)",
  "sample_movie_url": "[https://cc3001.dmm.co.jp/pv/MAwkRhEUIKm3Bpw46XbYlJ0632Em9cInMYE3mfoYX5LCf2mT97-mU28dgV_c5y/ssis00001_mhb_w.mp4](https://cc3001.dmm.co.jp/pv/MAwkRhEUIKm3Bpw46XbYlJ0632Em9cInMYE3mfoYX5LCf2mT97-mU28dgV_c5y/ssis00001_mhb_w.mp4)",
  "release_date": "2021-02-18",
  "duration": 147,
  "source_url": "[https://video.dmm.co.jp/av/content/?id=ssis00001](https://video.dmm.co.jp/av/content/?id=ssis00001)",
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
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-1.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-1.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-2.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-2.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-3.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-3.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-4.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-4.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-5.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-5.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-6.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-6.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-7.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-7.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-8.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-8.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-9.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-9.jpg)",
    "[https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-10.jpg](https://awsimgsrc.dmm.co.jp/pics_dig/digital/video/ssis00001/ssis00001jp-10.jpg)"
  ]
}
```
## 📡 数据来源
目前，本 API 仅提供来自 **[https://video.dmm.co.jp](https://video.dmm.co.jp)** 的部分精选视频元数据。

未来计划： 我们计划在未来的版本中增加对其他网站（如 [https://www.mgstage.com](https://www.mgstage.com)）的支持。

## ⚠️ 免责声明
内容警告： 本 API 提供有关成人内容的元数据。使用本 API 即表示您确认您在所在的司法管辖区已达到查看此类内容的法定年龄。

版权声明： 本 API 仅提供元数据索引服务。它不托管、分发或提供视频文件的下载链接。所有元数据权利和图片均属于其各自的版权所有者。

## 📄 许可证
本项目开源并遵循 MIT 许可证。
