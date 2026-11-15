# macOS phrase dictionary sources

`wiki_phrase_weights.dict.yaml` contains phrase-frequency/ranking data derived from the sources below. The table is offered under [CC BY-SA 4.0](https://creativecommons.org/licenses/by-sa/4.0/), with attribution to the listed Wikipedia revisions. The NAER frequency input is attributed separately under CC BY 4.0.

## Wikipedia training pages

Only the 29 training pages below contributed phrase counts. Article HTML snapshots are not stored in this repository. The revision ID links are permanent source references.

| Page | Revision | Source |
| --- | ---: | --- |
| 臺灣料理 | 95037830 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95037830) |
| 便利商店 | 94030184 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94030184) |
| 智慧型手機 | 95291946 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95291946) |
| 社群媒體 | 95380084 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95380084) |
| 臺灣文化 | 94963976 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94963976) |
| 臺灣教育 | 93830308 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93830308) |
| 臺灣氣候 | 93255494 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93255494) |
| 臺灣經濟 | 93837711 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93837711) |
| 臺灣歷史 | 95389568 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95389568) |
| 臺灣地理 | 95010991 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95010991) |
| 臺灣生態 | 94419959 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94419959) |
| 人工智慧 | 95531131 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95531131) |
| 網際網路 | 95486715 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95486715) |
| 健康 | 94044984 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94044984) |
| 金融 | 93005309 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93005309) |
| 日常生活 | 94513013 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94513013) |
| 人際溝通 | 91906533 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=91906533) |
| 家庭 | 95199253 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95199253) |
| 時間 | 94836537 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94836537) |
| 語言 | 95484300 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95484300) |
| 心理學 | 95544804 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95544804) |
| 旅遊 | 95448537 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=95448537) |
| 購物 | 94696705 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94696705) |
| 電子商務 | 93070321 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93070321) |
| 音樂 | 85238893 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=85238893) |
| 電影 | 93497843 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93497843) |
| 運動 | 93446240 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=93446240) |
| 睡眠 | 94196017 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94196017) |
| 職業 | 94953405 | [Wikipedia revision](https://zh.wikipedia.org/w/index.php?oldid=94953405) |

Wikipedia text is generally provided under CC BY-SA 4.0. The phrase table extracts 2–4 Han-character words and applies Dayi codes and frequency weights; it does not redistribute article HTML.

## NAER word-frequency prior

- Publisher: National Academy for Educational Research (NAER), *通用詞頻表*, final version 1141208.
- Official download page: [COCT downloads](https://coct.naer.edu.tw/page.jsp?ID=41).
- Source derivative and attribution: [ChiaKey Lexicon NAER frequency source](https://github.com/chiakich/ChiaKey-Lexicon/tree/dev/sources/naer-word-frequency).
- License: CC BY 4.0, as stated in the source-specific attribution notice. Source file SHA-256: `d8bf3ebec541c3dde967d536e05a33a2b8d5e4c4aeea1205feb4f0867220169a`.
- Transformation: use only supported 2–4 Han-character words with frequency at least 1 per million; use frequency as a phrase-ranking prior.

The dictionary was rebuilt using only the public `dayi2.dict.yaml` character codebook and `common_words_import.dict.yaml` from this repository. No userdb, personal phrase table, or local `mydayi_boost` file is included. TOCFL-only entries are excluded.
