# QATT Description Code – Specification

## 1. Syntax (BNF)

```text
<QATT-Code> ::= <Letter><Dot><Tone>  
<Letter>    ::= B | C | Ch | D | Dd | G | H | Kh | L | M | N | Ng | Nh | Ph | R | S | T | Th | Tr | V | X
<Dot>       ::= 0 | 1 | 2 | 3 | 4 | 5 | 6
<Tone>      ::= +1 | +2 | +3 | +4 | -1 | -2 | -3 | -4
<IDS>       ::= ⿰<QATT-Code><QATT-Code> | ⿱<QATT-Code><QATT-Code> | ⿲<QATT-Code><QATT-Code><QATT-Code> | ⿳<QATT-Code><QATT-Code><QATT-Code>
```

## 2. Components Overview (Table)

| Component | Syntax / Options | Notes |
|-----------|-----------------|-------|
| Letter    | `B, C | Ch | D | Dd | G | H | Kh | L | M | N | Ng | Nh | Ph | R | S | T | Th | Tr | V | X` | Base sign |
| Dot       | `0 | 1 | 2 | 3 | 4 | 5 | 6` | Placement on strokes |
| Tone      | `+1 | +2 | +3 | +4 | -1 | -2 | -3 | -4` | Corner placement (1=top-left … 4=bottom-left) |
| IDS       | `⿰<QATT-Code><QATT-Code> | ⿱<QATT-Code><QATT-Code> | ⿲<QATT-Code><QATT-Code><QATT-Code> | ⿳<QATT-Code><QATT-Code><QATT-Code>` | Ideographic sequences  

---

## 2. Component Meaning

1. **Letter** – Base sign from Quốc Âm Tân Tự  
2. **Dot Marking** – Optional dot, number indicates placement on strokes:
    - 1/2 → beginning/end of first stroke  
    - 3/4 → beginning/end of second stroke  
    - 5/6 → beginning/end of third stroke  
3. **Tone** – `+` = whole tone, `-` = half tone  
    - Number indicates corner: 1 = top-left, 2 = top-right, 3 = bottom-right, 4 = bottom-left  
4. **IDS** – Combines multiple QATT codes to represent complex characters

---

## 3. Examples

| QATT-Code  | Description                                        | SVG |
|------------|---------------------------------------------------|-----|
| Ch2-4      | Letter Ch, dot at end of first stroke (2), half tone top-left (-4) | ![Ch2-4](examples/Ch2-4.svg) |
| ⿱B1Kh4+3  | Combined character consisting of B1 on top of Kh4+3 | ![B1Kh4+3](examples/B1Kh4+3.svg) |

---

## 4. Notes
- QATT-DC describes **visual structure only**; no semantic meaning.  
- Extensible to new letters, dot positions, tones, and IDS sequences.
