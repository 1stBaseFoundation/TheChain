# pubMarker

A public repository whose only honest content is its language bar.

```
 93.4%  JavaScript
  4.2%  HTML
  1.3%  CSS
  0.4%  Java
  0.2%  PowerShell
  0.2%  PHP
  0.3%  Other
```

That is the exact composition of the private repo this one mirrors. The
code is not here. The bytes are.

## Why it is built this way

GitHub's language bar is computed by [Linguist](https://github.com/github-linguist/linguist):

1. **Extensions classify the file.** `.js` is JavaScript, `.html` is HTML,
   and so on. A file belongs to exactly one language.
2. **Bytes decide the percentage**, not lines. 934 bytes of JavaScript out
   of 1,000 total bytes is 93.4%.
3. **Some files are silently excluded** — vendored code, minified files,
   documentation (`.md`), and generated files.

So a breakdown can be forged with seven files totalling exactly 1,000
bytes. Ten bytes per tenth of a percent.

| Language   | Target  | File         | Bytes |
|------------|--------:|--------------|------:|
| JavaScript |  93.4 % | `index.js`   |   934 |
| HTML       |   4.2 % | `index.html` |    42 |
| CSS        |   1.3 % | `style.css`  |    13 |
| Java       |   0.4 % | `Main.java`  |     4 |
| PowerShell |   0.2 % | `script.ps1` |     2 |
| PHP        |   0.2 % | `index.php`  |     2 |
| Other      |   0.3 % | `mirror.awk` |     3 |

Everything else in this repo is invisible to the bar on purpose:
`README.md` is documentation, `.gitattributes` has no language, and
`tools/` is marked `linguist-vendored`.

## Keeping it honest

```
pwsh -File tools/verify.ps1
```

Recomputes the breakdown from disk and fails if a single byte drifts.

## The point

Open source is sold as a commons. It is closer to a plantation with a
public API: the maintainer tills, the corporation harvests, and the
license is the deed nobody ever reads.

Cyber slavery does not arrive in chains. It arrives as a green square.
As a stranger's issue at 2 a.m. As "quick question" in your mentions.

A mirror keeps no secrets and holds no opinion of its own. It only
refuses to distort the shape of the thing standing in front of it.

The bytes are real. The work is not.