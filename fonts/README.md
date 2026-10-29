# TSD Sans web subsets

Source family: Noto Sans CJK SC, © 2014–2021 Adobe. Licensed under SIL OFL 1.1; see OFL.txt. Original copyright and family metadata remain in each font.

Official source and license: https://github.com/notofonts/noto-cjk/tree/main/Sans

The website uses WOFF2 subsets for Regular (400), Medium (500) and Bold (600–700 role mapping). Coverage includes GB2312, Latin, punctuation, and current site text. Uncovered characters fall back to the system font. font-display:swap keeps content readable while downloading; the three files total about 7.57 MB and are browser-cacheable.

Rebuild with Python fonttools[woff], HarfBuzz hb-subset, and the three original NotoSansCJKsc OTF files:

    python3 scripts/build-font-subsets.py --font-dir /path/to/original-fonts

Run from the project root after adding text that requires additional glyphs. manifest.json records source and subset hashes.
