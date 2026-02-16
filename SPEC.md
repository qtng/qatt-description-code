# QATT Description Code – Specification

Version: 0.1 preliminary

## 1. Syntax (BNF)

```text
<QATT-Code> ::= <Letter><Dot><Tone>  
<Letter>    ::= B | C | Ch | D | Dd | G | H | Kh | L | M | N | Ng | Nh | Ph | R | S | T | Th | Tr | V | X
<Dot>       ::= 0 | 1 | 2 | 3 | 4 | 5 | 6 | •0 | •1 | •2 | •3 | •4 | •5 |• 6
<Tone>      ::= +1 | +2 | +3 | +4 | -1 | -2 | -3 | -4
<IDS>       ::= ⿰<QATT-Code><QATT-Code> | ⿱<QATT-Code><QATT-Code> | ⿲<QATT-Code><QATT-Code><QATT-Code> | ⿳<QATT-Code><QATT-Code><QATT-Code>
```

## 2. Components Overview (Table)

| Component | Syntax / Options | Notes |
|-----------|-----------------|-------|
| Letter    | B, C, Ch, D, Dd, G, H, Kh, L, M, N, Ng, Nh, Ph, R, S, T, Th, Tr, V, X | Base sign (cán tự) |
| Dot (in QATT order) | 0, 1, 2, 3, 4, 4, 6 | Placement of dot in QATT order |
| Dot (in stroke oder) | •0, •1, •2, •3, •4, •5, •6 | Placement on strokes |
| Tone (thanh điệu) | +1, +2, +3, +4, -1, -2, -3, -4 | plus sign for full tone symbol "ₒ", minus sign for half tone symbol "꜀", number designates corner placement (1=top-left … 4=bottom-left) |
| IDS       | ⿰, ⿱, ⿲, ⿳ | Ideographic sequences  

---

## 2. Component Meaning

1. **Base Symbol** – Base symbol (cán tự) from Quốc Âm Tân Tự, the symbol name is case sensitive, i.e. first letter is uppercase and subsequent letters are lowercase.  
2. **Dot Marking** – Optional dot (phẩy), the number indicates placement of dot. If the number is preceeed by a "•", the number indicates the order according to the original QATT instructions from the 19th century. Otherwise the number indicates the placement on **rectangle strokes** or **support stroke**. Here **rectangle strokes** are the outermost parallel strokes of a character or the crossing strokes if no parallel strokes exist in a character. The corners of the rectangle or parallelogram formed by the rectangle strokes provide the placement positions 1 to 4 in clockwise order, while the remaining **support stroke** provides the placement positions 5 and 6:
   * 1: placement on top left of rectangle strokes
   * 2: placement on top right of rectangle strokes
   * 3: placement on bottom right of rectangle strokes
   * 4: placement on bottom left of rectangle strokes
   * 5: placement on start of support stroke
   * 6: placement on send of support stroke
3. **Tone** – `°` = whole tone symbol (thanh điệu dương), `꜄` = half tone symbol (thanh điệu âm)
    - Number indicates corner: 1 = top-left, 2 = top-right, 3 = bottom-right, 4 = bottom-left  
4. **IDS** – Combines multiple QATT codes to represent complex characters

---

## 3. Examples

| QATT-Code  | Description                                        | SVG |
|------------|---------------------------------------------------|-----|
| Tr1+8 or Tr•1+8 | Base symbol Tr (廾) with dot in first position according to QATT, i.e. begin of first stroke, and half tone symbol at position 4 (bottom-left) | ꜀升 |
| Dd1+1 or Dd•3+1 | Base symbol Dd (士) with dot in first losition according QATT, i.e. at start of second stroke, and full tone symbol at position 1 (top-left) | ⁰壬 |
| ⿱ThDd-2 | Combined character consisting of unmarked Th on top of Dd with half tone symbol at position 2 (top-right) | 芏꜄ |茱

---

## 4. Notes
- QATT Description Code describes **visual structure only**; no semantic meaning.  
- Extensible to new letters, dot positions, tones, and IDS sequences.

## 5. Reference Table

Reference table with dot positions in stroke order.

![QATT Lookup Table](qatt.png)
