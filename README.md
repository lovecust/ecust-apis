# Apis of Ecust

## about-apis

server: http://apis.lovecust.com

## Ecust APIs

- Ecust JWC Newses
	- [*GET* Ecust JWC Newses List][api-ecust-jwc-newses]
	- JWC News
		- [*GET* JWC News Detail][api-ecust-jwc-news]
		- Ecust JWC News Detail
			- [*GET* JWC News Comments List][api-ecust-jwc-news-comments]
			- *POST* a News Comment
- Ecust Library
	- [*GET* Library Status][api-ecust-library-status]
	- Library Status Statistics
		- [*GET* Library Status Statistics][api-ecust-library-status-statistics]

## api-details

---

- [library-status][api-ecust-library-status]

```
# students number of library

params:
return:
	today: <int>
	occupied: [int]
	available: [int]
```
example:
```json
{
  "today":3200,
  "available": [4, 61, 112, 80, 78, 2],
  "occupied": [32, 261, 349, 292, 271, 54]
}
```
---
- [jwc-list][api-ecust-jwc-newses]

```

# jwc latest news list

params:
return:
	[
		url: <string>  # "/path/link/file.htm"
		name: <string>
		date: "2016-04-05"
	]
```

example:

```json
[
  {
    "url": "/s/75/t/134/09/b1/info68017.htm",
    "name": "20161学期选课手册下载",
    "date": "2016-06-06",
    "tag": 1,
    "bold": true,
    "md5": "ddfc855bcf25cf1805b0fb87d46158da"
  }, {
    "url": "/s/75/t/134/08/19/info67609.htm",
    "name": "端午节放假通知",
    "date": "2016-05-23",
    "tag": 1,
    "md5": "4a6b2154f28c60e3eddc2070f2bb2feb"
  }
]
```

[api-ecust-jwc-newses]: http://apis.lovecust.com/apis/ecust/jwc/newses "API: Get Ecust Newses List"
[api-ecust-jwc-news]: http://apis.lovecust.com/apis/ecust/jwc/newses/29ba220583cae79ff0005e8804d676ab "API: Get Ecust JWC News Detail"
[api-ecust-jwc-news-comments]: http://apis.lovecust.com/apis/ecust/jwc/newses/29ba220583cae79ff0005e8804d676ab/comments "API: Get JWC News Comments"
[api-ecust-library-status]: http://apis.lovecust.com/apis/ecust/library/status "API: Get Ecust Library Status"
[api-ecust-library-status-statistics]: http://apis.lovecust.com/apis/ecust/library/status/statistics?interval=1&limit=100 "API: Get Library Status Statistics"
