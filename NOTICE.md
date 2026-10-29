# Notice

Your own contributions to this repository — new rows, your own changes to existing rows, translations, notes, documentation — are released under [CC0 1.0](LICENSE): no rights reserved, so anyone may use them for any purpose, including Nôm Na Việt itself. Where you correct a pre-filled row, only your change is CC0; any third-party content it builds on keeps the terms listed below.

Some files are pre-filled from third-party sources so that you can see what is missing. That pre-filled data is **not** covered by CC0 and stays under its original terms:

- `classifications/character-classifications.csv` — the A1–G2 codes already filled in (about 7,700 rows) come from Nguyễn Quang Hồng, *Tự Điển Chữ Nôm Dẫn Giải* (NXB Khoa học Xã hội, 2014), via [Digitizing Vietnam](https://www.digitizingvietnam.com). The code system itself is his.
- `decompositions/partial-decompositions.csv` — the `CurrentIDS` column is derived from `ids.txt` in [cjkvi-ids](https://github.com/cjkvi/cjkvi-ids), which is derived from the [CHISE project](http://www.chise.org/) and follows its terms; the rest of cjkvi-ids is GPLv2. A copy of the GPLv2 is in [`licenses/GPL-2.0.txt`](licenses/GPL-2.0.txt).
- Character metadata — the `unicode`/`Unicode`, `stroke_count`/`StrokeCount` and `radical`/`Radical` columns, wherever a CSV under `classifications/`, `decompositions/` or `variants/` has them — draws on the [Unihan Database](https://www.unicode.org/charts/unihan.html), under the Unicode License. Its copyright and permission notice is in [`licenses/Unicode.txt`](licenses/Unicode.txt).
