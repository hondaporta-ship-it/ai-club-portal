# 新しいアプリを追加するには

**HTMLは一切触らなくていい。`apps.json` だけ編集してpushするだけ。**

---

## 手順

1. `apps.json` を開く
2. `"works"` 配列に1エントリ追加する
3. `git add apps.json && git commit -m "Add: アプリ名" && git push`
4. 1〜2分後にポータルに自動反映 ✅

---

## apps.json の書き方

```json
{
  "id": "repo名（ユニークなID）",
  "title": "アプリ名",
  "icon": "絵文字1個",
  "category": "fun または useful",
  "url": "https://hondaporta-ship-it.github.io/repo名/",
  "by": "作った人の名前 または AI同好会",
  "description": "一言説明（任意）"
}
```

### category の使い分け

| category | 意味 |
|----------|------|
| `"fun"` | おふざけ系・エンタメ系 |
| `"useful"` | 役に立つ系・業務系 |

---

## 例：新アプリ「シフト計算機」を追加する場合

```json
{
  "id": "shift-calc",
  "title": "シフト計算機",
  "icon": "📅",
  "category": "useful",
  "url": "https://hondaporta-ship-it.github.io/shift-calc/",
  "by": "樫迫さん",
  "description": "警備シフトの工数を自動計算"
}
```

---

## ルール

- `id` はそのままGitHub Pagesのリポジトリ名に合わせると管理しやすい
- アプリのリポジトリが公開されていて、GitHub PagesでURLが生きていること
- `icon` は絵文字1個だけ（ページの見た目が崩れるので）
- 作者不明なら `"by": "AI同好会"` でOK

---

## ポータルURL

https://hondaporta-ship-it.github.io/ai-club-portal/
