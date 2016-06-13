# Apis of Ecust

## about-apis
server: http://apis.lovecust.com
path: /apis/ecust-related/<api-specific-name>

## api-summary
0. ecust-library-status
0. ecust-jwc-list

## api-details
---
- [ecust-library-status](http://apis.lovecust.com/apis/ecust-related/ecust-library-status)
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
- [ecust-jwc-list](http://apis.lovecust.com/apis/ecust-related/ecust-jwc-list)

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
