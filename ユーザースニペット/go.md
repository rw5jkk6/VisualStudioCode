## 徹底解説VScode  cf183

- 左下の管理(歯車の絵)からユーザースニペットを選ぶ,go.jsonと入力する
- 次に下の線以下をコピーして、貼り付ける
- これで.goファイルでstartと入力したら、自動で入力できる


```json
{
	"package main":{
		"scope":"go",
		"prefix": "start",
		"body": [
			"package main",
			" ",
			"import (",
			"   \"fmt\"",
			")",
			"",
			"func main(){$1",
			"}"

		]
	}
}
```
