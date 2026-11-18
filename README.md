# nomnaviet-contrib

Community contributions to [Nôm Na Việt (喃哪越)](https://nomnaviet.com/vi) — a platform for Vietnamese Hán Nôm studies.

This repo is the **canonical source** for translations and the **staging area** for character data contributions. Maintainers periodically sync changes back into the main app.

## What's here

| Folder | What | How to contribute |
|---|---|---|
| [`i18n/`](./i18n/) | UI translation files (vi, en, fr, zh) | See [`i18n/README.md`](./i18n/README.md) |
| [`decompositions/`](./decompositions/) | Character component data (IDS) | See [`decompositions/README.md`](./decompositions/README.md) |
| [`classifications/`](./classifications/) | A1–G2 character formation classifications (Nguyễn Quang Hồng, *Tự Điển Chữ Nôm Dẫn Giải*, 2014) — ~18,000 of 25,827 characters still blank | See [`classifications/README.md`](./classifications/README.md) |
| [`variants/`](./variants/) | Unicode-codepoint dị thể (異體字) pairs — same Vietnamese word, different codepoint. Strong gap for pure-Nôm chars (2.3% coverage) since Unihan is Sinophone-centric. | See [`variants/README.md`](./variants/README.md) |

More content areas may be added later (e.g. historical dictionary digitization).

### Characters written as a sequence

Some Nôm characters are written as a base character plus a variation selector (U+E0100–E01EF) or the cá/nháy reading mark (U+16FF0/U+16FF1), NOM Foundation's standard form for many characters NomNaTong used to keep in its Private Use Area. Such a character is one character, so in these CSVs its `Character` cell holds the whole sequence and its `Unicode` cell lists every codepoint, space-separated: `U+4E99 U+16FF0`. Its stroke count and radical are those of the glyph it names, which can differ from its base character's (a variant glyph can have a stroke more or less). Keep the sequence together when you edit, a spreadsheet that drops the invisible selector turns it into a different character.

## How to contribute

If you're new to GitHub:

1. Click the **Fork** button at the top right of this page.
2. Edit files directly in your fork's web UI (pencil icon on any file).
3. Click **Propose changes** → **Open pull request**.

If you're comfortable with git:

```bash
git clone https://github.com/<your-username>/nomnaviet-contrib.git
cd nomnaviet-contrib
# edit files
git add . && git commit -m "fix: ..." && git push
# then open a PR on GitHub
```

No need to run any code or set up an environment — these are plain JSON and CSV files.

## License

Contributions are released under [CC0 1.0](LICENSE) (public domain dedication). By submitting a PR you confirm the contribution is your own work, or that you have the right to release it under CC0, and you agree it may be incorporated into the Nôm Na Việt app.

Data that was pre-filled from third-party sources keeps its original terms. See [NOTICE.md](NOTICE.md) for which files and columns that covers.

## Questions

Open an [Issue](../../issues) or email hello@nomnaviet.com.
