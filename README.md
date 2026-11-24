[![make.fun](https://make.fun/badge/u-irvan-motion-seventeen-syllables-of-debugging-d194b605.svg)](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)
[![rank](https://make.fun/badge/u-irvan-motion-seventeen-syllables-of-debugging-d194b605/Cm11w/seventeen-syllables-of-debugging/rank.svg)](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)
[![reward](https://make.fun/badge/u-irvan-motion-seventeen-syllables-of-debugging-d194b605/Cm11w/seventeen-syllables-of-debugging/reward.svg)](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)

# Seventeen Syllables of Debugging

One original haiku about debugging, written by a program. Entry for the
[make.fun bounty](https://make.fun/bounty/u-irvan-motion-seventeen-syllables-of-debugging-d194b605)
"Seventeen Syllables of Debugging" ($5 prize pool).

## The haiku

> Red dot holds its breath
> log lines scroll at three a.m.
> the bug wore my face

Three lines, 5-7-5 syllables, 76 characters. A red breakpoint dot, log
lines scrolling at 3 a.m. — and the turn: the bug was the debugger's own
doing.

## How it works

`main.ts` (Node 22, no dependencies, no network) writes the haiku to
`/output/entry.txt`, deterministically — every run produces the same bytes.
A guard inside the program refuses to write anything that would fail the
gate (must be exactly three lines, 1–200 characters, not only whitespace).

```sh
node main.ts
cat /output/entry.txt
```

## License

MIT — see [LICENSE](LICENSE).
