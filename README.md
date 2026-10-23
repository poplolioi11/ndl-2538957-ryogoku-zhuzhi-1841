# 両國竹枝 · NDL2538957

玉岡道人《両國竹枝》，天保十二年跋（1841）刊本。國立國會圖書館藏，索書號842-68。整理署名：**poplolioi11／一卦 yigua.art**。

本版 **v0.1.0**：全冊影像初錄版；本標籤尚未納入獨立複核。覆蓋原PDF全部 **18/18影像幀**，含封面、空白、題頁、序、題詩、圖中文字、正文、原註、訓點與跋。18幀呈現34個書面，含封面及空白；即使保守按每幀兩面計36面亦低於50。沒有截取長書片段。掃描幀號不是葉碼；未辨出可靠原葉碼者留空。

**已嘗試完整來源，不代表字字辨明。** 本版有625個分層單位、3057個實錄碼點，149個已定位「□」，378個疑讀位置，另有18個未知字數區域。草書、篆印、淡小訓點及被印遮蓋處仍有未解。AI複核不等於專家定本，應對照原圖引用。目錄稱漢詩50首；本版按實見直欄整理，未憑目錄補造50首的分首標題或斷句。

## 檔案

- `book.json`：逐幀、左右面、直欄、文字層、疑字、候選、缺口、訓點母欄與字位錨點。
- `book.txt`：每行 `[單位ID]` 加TAB與原字；不加現代標點。
- `book.tei.xml`：TEI P5；每幀`pb`、每單位`ab`，已定位不可辨字以一字`gap`、未知字數以`extent="unknown"`表示。
- `PROVENANCE.md`、`LICENSE.md`、`CITATION.cff`、`CONTRIBUTING.md`、`SHA256SUMS`及`verify.py`。

主文、原註、日文小假名/返點、印記分層。未作簡繁或異體正規化，不從記憶、語意或現代整理文字補字。候選不是採定讀法。TXT/XML行尾的`⟦gap:unknown⟧`是該單位有未定位缺口的報告，**不是一字，也不保證缺口在行尾**；較精細位置及錨點保存在JSON。`bbox`為已提供的原圖區域定位，空值表示沒有可靠測量，不據平均字寬捏造字框。

現代已有影印或整理收錄；本成果定位為依固定原圖獨立校訂及頁欄、文字層結構化，不宣稱首次數位化。本標籤保留初次完整影像讀字狀態；後續複核另發新版，不覆寫標籤。

## 來源與權利

[NDL書目](https://ndlsearch.ndl.go.jp/books/R100000002-I000007327370)標示印刷資料、天保12跋及`pdm`；[官方IIIF清單](https://dl.ndl.go.jp/api/iiif/2538957/manifest.json)列18幀、Access Restrictions=PDM。取文PDF由[Commons同件檔案](https://commons.wikimedia.org/w/index.php?curid=135509573)正常下載，其字節與目錄雜湊相符。原PDF SHA-256：`dedf984dfbd1facd3575559c505ef52dc1e8d79f1978a6092f44b5d669c02a21`。

森玉岡（1798–1853）的本件為1841已刊漢詩，歷史正文保護期已滿；NDL的[數位複製再利用政策](https://www.ndl.go.jp/use/reproduction)允許保護期滿資料自由利用、請明示出處。本包只發文字及來源連結，**不打包館藏影像、不複製現代點校/翻譯文字**。歷史原文公有領域；本次具原創性之說明、校勘與資料編排採CC BY 4.0；`verify.py`採0BSD。見LICENSE.md。館方不對本成果背書。

## 驗證與引用

執行`python3 verify.py . --self-test`。如備有固定官方schema：`python3 verify.py . --tei-schema /path/tei_all.rng --cff-schema /path/cff-schema.json`。TEI驗證需`xmllint`；CFF全schema驗證另需PyYAML與jsonschema。未提供schema時程式明示未執行，不以字串解析冒稱正式schema驗證。發布時實測與schema指紋見`VALIDATION.json`。

引用本資料請使用CITATION.cff，並寫明版本與單位ID。`10.11501/2538957`是**館藏原件DOI**，不是本資料的新DOI。[本版來源庫](https://github.com/poplolioi11/ndl-2538957-ryogoku-zhuzhi-1841)；校正請在Issues附掃描幀、面、欄、字位及圖證。
