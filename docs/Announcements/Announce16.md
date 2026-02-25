# 🔥【テスト】お知らせ配信・完全版 Markdown 検証カード

アプリのお知らせ機能が **どこまで Markdown を解釈できるか** を確認するための総合テストメッセージです。

---

## 1. 見出しテスト

# H1 見出し  
## H2 見出し  
### H3 見出し  
#### H4 見出し  
##### H5 見出し  
###### H6 見出し

---

## 2. 強調・インライン装飾テスト

- **太字**
- *斜体*
- ***太字＋斜体***
- ~~取り消し線~~
- `インラインコード`
- <span style="color: red; font-weight: bold;">HTML カラー文字</span>  
- <span style="background: #fff3cd; padding: 2px 4px; border-radius: 4px;">ハイライト</span>

---

## 3. リンク・画像テスト

**リンク：**  
[https://example.com](https://example.com)

**画像（外部 URL）：**  
※ WebView2 の CSP によってはブロックされる可能性あり  
```
![テスト画像](https://via.placeholder.com/150)
```

---

## 4. 引用テスト

> これは引用です  
>> これは二重引用です

---

## 5. リストテスト

### ● 箇条書き
- りんご
- みかん
  - ネーブル
  - デコポン
- ぶどう

### ● 番号付き
1. ステップ1
2. ステップ2
3. ステップ3

### ● チェックボックス
- [x] 完了したタスク
- [ ] 未完了タスク
- [ ] 進行中タスク

---

## 6. コードブロックテスト

```csharp
public class Test {
    public void Run() {
        Console.WriteLine("Hello Markdown!");
    }
}
```

```json
{
  "name": "V-Shift",
  "version": "1.0.0",
  "status": "test"
}
```

---

## 7. 表テスト

| 種類 | 値 | 備考 |
|------|------|------|
| CPU | 3.2GHz | OK |
| RAM | 16GB | 推奨 |
| Storage | 512GB | SSD |

---

## 8. 折りたたみ（details）テスト

<details>
<summary>クリックして展開</summary>

ここに折りたたみ内部のテキストが入ります。  
HTML の `<details>` は Markdig でそのまま動作します。

- 内部リスト
- 内部テキスト

</details>

---

## 9. 数式（LaTeX）テスト

インライン：  
\(\sqrt{3x-1} + (1+x)^2\)

ブロック：  
\[
E = mc^2
\]

---

## 10. 絵文字テスト

- 😀 😎 🎉 🚀  
- 👍 ❗ ✔️ ✨

---

## 11. 脚注テスト

これは脚注付きテキストです`[この結果は、表示するには安全でなかったようです。切り替えて、別のことを試してみましょう!]`。


---

## 12. 水平線テスト

---
***
___

---

## 13. HTML 埋め込みテスト

<div style="padding: 10px; border: 1px solid #ccc; border-radius: 6px;">
  <strong>HTML ボックス</strong><br>
  ここは HTML がそのまま描画される領域です。
</div>

---

## 14. 絵文字＋強調＋リンクの複合

**🚀 重要：**  
[サーバーステータスはこちら](https://example.com/status) を確認してください。

---

## 15. 最後に：メタ情報

配信日時：2026-02-25 21:00  
配信元：システム（テスト）