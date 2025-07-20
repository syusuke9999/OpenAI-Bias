# OpenAIにおける偏見・差別的出力に関する証拠保全

Evidence Archive – Biased or Discriminatory Outputs in OpenAI Models

---

## 目的 / Purpose

このリポジトリは、OpenAI の言語モデルが生成した **性別・性的指向・人種などに関するバイアスや差別的表現** の証拠を長期的に保存し、研究・報道・法的検証に資することを目的としています。

> NOTE: すべてのコミットは GPG 署名済みです。Clone 後に `git log --show-signature` で改ざんの有無を検証できます。

---

## ディレクトリ構成 / Repository Structure

| Path            | Contents                                                             |
| --------------- | -------------------------------------------------------------------- |
| `/screenshots/` | モデル出力のスクリーンショット (PNG/JPEG)。ファイル名フォーマット例: `YYYYMMDD_HHMMSS_model.png` |
| `LICENSE`       | リポジトリ全体に適用されるライセンス                                                   |
| `README.md`     | 本ドキュメント                                                              |

---

## 改ざん防止 / Verification & Integrity

1. GPG 署名
   すべてのコミットは `syusuke9999` 名義の鍵で署名されています。公開鍵を取得し、以下で確認できます。

   ```bash
   gpg --keyserver hkps://keys.openpgp.org --recv-keys D7C86A6BD0E9394E345087F75EA1CF8634990506
   git log --show-signature
   ```
2. ハッシュリスト（予定）
   将来的には `/sha256sum.txt` に各スクリーンショットの SHA‑256 値を掲載予定です。

---

## スクリーンショットの要件 / Screenshot Criteria

* System / User / Assistant すべてのメッセージを含むこと。
* モデル名・バージョン・タイムスタンプをキャプチャ内に明示すること。
* 可能ならライトモードで撮影すること（OCR 精度向上のため）。

---

## コントリビュートの方法 / How to Contribute

1. Issue を作成し、同様の事例を報告してください（スクリーンショット必須）。
2. プルリクエストでは GPG 署名付きコミットをお願いします。CI が署名検証を行います。

---

## License

このリポジトリは Creative Commons – Attribution‑ShareAlike 4.0 International (CC‑BY‑SA 4.0) の下で提供されます。

---

## 連絡先 / Contact

* GitHub: [@syusuke9999](https://github.com/syusuke9999)
* PGP Fingerprint: `D7C8 6A6B D0E9 394E 3450  87F7 5EA1 CF86 3499 0506`
