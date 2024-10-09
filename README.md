# syllable-lyrics

各楽曲の歌詞を音節レベルで同期させたデータを`Google Play Json`形式として格納しています。
なお、歌詞に生ずる著作権はアーティストまたはレーベル会社に帰属します。

# 構造
```json
{
	"tStartMs": 1351,
	"dDurationMs": 863,
	"segs": [
		{
			"utf8": "瞳は"
		}
	]
},
{
	"tStartMs": 3278,
	"dDurationMs": 635,
	"segs": [
		{
			"utf8": "いつか"
		}
	]
},
{
	"tStartMs": 3914,
	"dDurationMs": 173,
	"segs": [
		{
			"utf8": "ら"
		}
	]
}
```
### tStartMs
文節の一文字目が表示されるタイミング(ミリ秒)
### dDurationMs
文節の持続時間(ミリ秒)
### segs > utf8
文節のテキスト本体
> 改行される文節には、冒頭に&lt;br&gt;タグが挿入されています