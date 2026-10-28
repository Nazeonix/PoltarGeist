# PoltarGeist

**PoltarGeist** is an experimental type project exploring a compact, balanced reading experience for Latin and Cyrillic text, based on the open-source Geist and Inter typefaces.

> **Status:** Experimental. Please test the font in your own applications and report spacing, kerning, or glyph issues.

## Goals

- Improve the visual balance of Latin and Cyrillic text together.
- Explore tighter, more consistent spacing for Cyrillic text.
- Keep the clean, contemporary feel of the source typefaces.
- Make the font easy to install and test on desktop Linux and other systems.

## Typeface origins

PoltarGeist is derived from or combines work from these upstream projects:

- **Geist** — https://github.com/vercel/geist-font
- **Inter** — https://github.com/rsms/inter

The original projects and their authors retain their respective rights. See [`OFL.txt`](OFL.txt) for the applicable license text and copyright notices.

## Installation on Arch Linux

1. Download the font files from the repository or a release archive.
2. Copy the `.ttf` files into a user font directory, for example:

   ```bash
   mkdir -p ~/.local/share/fonts/PoltarGeist
   cp ./*.ttf ~/.local/share/fonts/PoltarGeist/
   fc-cache -f
   ```

3. Check that Fontconfig can find the family:

   ```bash
   fc-match "PoltarGeist"
   ```

4. Select **PoltarGeist** in the font picker or application settings.

If the font files are stored in a subdirectory, adjust the `cp` command to match their location.

## Test text

Use these strings to check the appearance and coverage of Latin and Cyrillic glyphs:

```text
The quick brown fox jumps over the lazy dog.
Привіт, Україно! Ґґ Єє Іі Її
Симетрія · Типографіка · читабельність
Бб Дд Жж Йй Цц Щщ Љљ Њњ Ћћ Џџ
```

Character support depends on the actual glyphs included in the font files. This test text does not guarantee that every character is present.

## Feedback and contributions

Please open an issue with:
- the operating system and application,
- the exact text that looks incorrect,
- a screenshot if possible,
- the font file and style used.

Useful areas for review include Cyrillic side bearings, kerning pairs, diacritics, punctuation, and consistency between Latin and Cyrillic glyphs.

## License

PoltarGeist font software and derivatives must be distributed under the applicable SIL Open Font License, Version 1.1, subject to its terms. The original Geist and Inter copyright notices must be preserved. Read [`OFL.txt`](OFL.txt) before redistributing or modifying the font files.

This project is unofficial and is not affiliated with or endorsed by the Geist or Inter project maintainers.
