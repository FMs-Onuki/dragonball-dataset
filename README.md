# Dragon Ball Character Dataset

ドラゴンボールキャラクターの仙豆摂取回数・復活回数をまとめた非公式データセットです。

## 免責事項

原作『ドラゴンボール』の正史（鳥山明の漫画、および公認範囲のアニメ版）に基づき当プロジェクトが独自に集計した非公式データです。映画・GT・アニメオリジナル回など正史外の描写は集計対象外です。`senzu_beans_eaten` の`9999`（ヤジロベー）は「1位だが具体的な数は非公開」という公式発表を表す象徴的な値です。

## データ

[`data/characters.json`](data/characters.json)

| フィールド | 説明 |
| --- | --- |
| `name` / `reading` | キャラクター名 / 読み仮名 |
| `birth_year` / `death_year` | 生誕年・死亡年（Age表記）。不明・存命の場合は `null` |
| `senzu_beans_eaten` | 作中で摂取した仙豆の回数（公式発表分のみ）。未発表は `null` |
| `revival_count` | 正史における死亡→復活の回数 |

## ライセンス

MIT License（本リポジトリのコード・構成に適用）。データ自体（キャラクター名・設定等）の著作権は『ドラゴンボール』作者および関連企業に帰属します。

## 出典

原作本編・公式X投稿（一次情報）の内容は、それを報じた記事・Wiki（二次情報）経由で把握しており、原典そのものは未閲覧です（孫引き）。原典に直接あたりたい場合は二次情報源の出典表記を辿ってください。

### 一次情報（原典）

| フィールド | 原典 |
| --- | --- |
| `name` / `reading` | 原作『ドラゴンボール』（鳥山明、集英社） |
| `senzu_beans_eaten` | Dragon Ball公式X（[@DB_official_jp](https://x.com/DB_official_jp/status/1489071158305636356)、2022-02-04投稿） |
| `birth_year` / `death_year` / `revival_count` | 原作漫画・アニメ版『Z / 超』本編（正史） |

### `revival_count` の内訳（正史）

| キャラクター | 回数 | 死亡イベント |
| --- | --- | --- |
| 孫悟空 | 2 | ラディッツ戦／セルゲームズ（自己犠牲、7年後に復活） |
| ベジータ | 2 | フリーザ戦（ナメック星）／魔人ブウ戦（自爆） |
| ヤジロベー | 1 | 魔人ブウの地球破壊 |
| ピッコロ | 2 | ナッパ戦（グレゴリーを庇う）／魔人ブウの地球破壊 |
| クリリン | 3 | タンバリンに殺害／フリーザに殺害／魔人ブウの地球破壊 |
| セル | 0 | セルゲームズで死亡後、未復活 |
| ビーデル | 1 | 魔人ブウの地球破壊 |
| フリーザ | 2 | 未来トランクスに討たれ復活（復活のF）／力の大会参加のためゼノンにより復活（後に恒久化） |
| ヤムチャ | 2 | サイバイマンの自爆に巻き込まれ死亡／魔人ブウの地球破壊 |
| 孫悟飯 | 1 | 魔人ブウの地球破壊 |
| 天津飯 | 2 | 気功砲を放ち力尽きて死亡／魔人ブウの地球破壊 |
| 餃子 | 3 | ピッコロ大魔王に殺害／ナッパへの自爆特攻／魔人ブウの地球破壊 |
| 亀仙人 | 2 | ピッコロ大魔王に殺害／魔人ブウの地球破壊 |
| 人造人間17号 | 2 | セルに吸収され自爆に巻き込まれ死亡／魔人ブウの地球破壊（力の大会でのジレン戦の自爆は生存確認済みのため未カウント） |

### `birth_year` / `death_year` の根拠

| キャラクター | `birth_year` | `death_year` |
| --- | --- | --- |
| 孫悟空 | Age 737 | null（生存中） |
| ベジータ | Age 732 | null（生存中） |
| ヤジロベー | Age 735 | null（生存中） |
| ピッコロ | Age 753 | null（生存中） |
| クリリン | Age 736 | null（生存中） |
| セル | null（生誕年の記載なし） | Age 767（セルゲームズで死亡、未復活） |
| ビーデル | null（二次情報源に記載なし） | null（生存中） |
| フリーザ | null（二次情報源に記載なし） | null（生存中、力の大会後に復活が恒久化） |
| ヤムチャ | Age 733 | null（生存中） |
| 孫悟飯 | Age 757 | null（生存中） |
| 天津飯 | Age 733 | null（生存中） |
| 餃子 | null（二次情報源に記載なし） | null（生存中） |
| 亀仙人 | Age 430 | null（生存中） |
| 人造人間17号 | null（改造年のみ判明） | null（生存中） |

`birth_year`はDragon Ball Encyclopedia年表、`death_year`（セル）はKanzenshuu年表に基づきます（下表参照）。

### 参照した二次情報源

| サイト名 | 記事 | 最終アクセス日 |
| --- | --- | --- |
| CBR | [Who Has Eaten the Most Senzu Beans](https://www.cbr.com/dragon-ball-senzu-beans-goku-vegeta-yajirobe/) | 2026-08-19 |
| CBR | [Most Resurrections, Ranked](https://www.cbr.com/dragon-ball-characters-most-least-resurrections/) | 2026-08-19 |
| Dragon Ball Encyclopedia | [List of birth dates](https://dragonballencyclopedia.com/wiki/List_of_birth_dates) | 2026-08-19 |
| Dragon Ball Fandom Wiki | [End of Earth](https://dragonball.fandom.com/wiki/End_of_Earth) | 2026-08-19 |
| ScreenRant | [Characters Who've Died And Come Back The Most](https://screenrant.com/dragon-ball-characters-who-died-revived-most/) | 2026-08-19 |
| Kanzenshuu | [Dragon Ball Timeline](https://www.kanzenshuu.com/wiki/Dragon_Ball_Timeline) | 2026-08-19 |

本プロジェクトはDragon Ball公式・上記各サイトの運営会社とは提携・関係がなく、公認・承認を受けたものでもありません。各名称・商標は各権利者に帰属します。
