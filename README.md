# QATT Description Code  
*Mã mô tả QATT*

## Motivation

The **QATT Description Code (QATT-DC)** is a compact symbolic notation used to describe the **visual and structural form** of Quốc Âm Tân Tự signs.  
Since these signs are not currently encoded in Unicode, QATT-DC provides a consistent and reproducible way to support discussion, analysis, and publication.

**Mã mô tả QATT (QATT Description Code)** là một hệ thống ký hiệu ngắn gọn dùng để mô tả **cấu trúc hình thức** của các ký hiệu *Quốc Âm Tân Tự*.  
Do các ký hiệu này hiện chưa được mã hóa trong Unicode, QATT-DC cung cấp một phương tiện thống nhất để **thảo luận, phân tích và dẫn chiếu** trong các tài liệu học thuật và kỹ thuật.

## Scope
- Describes **visual structure only**.  
- Does **not define Unicode code points** or character identity.  
- Supports scientific discussions and referencing.

## QATT-DC Code
- **Letter Symbol**: e.g. `B`, `C`, `Ch`, `D`, `Dd`
- **Dot Marking**: `0` = no dot, `1–6` = dot added
  - Number indicates placement on strokes:
    - 1/2 → beginning/end of first stroke
    - 3/4 → beginning/end of second stroke
    - 5/6 → beginning/end of third stroke
- **Tone Symbol**: `+1` to `+4` for whole tone symbol, `-1` to `-4` for half tone symbol  
  - Number indicates placement: 1 = top-left, 2 = top-right, 3 = bottom-right, 4 = bottom-left
- **IDS (Ideographic Description Sequence)**: Combine multiple QATT codes to represent complex characters, e.g. ⿱C1D6+4, ⿱G3H2-1

**Example**:  
- `Ch2-4` → Letter symbol `Ch`, dot at end of first stroke (2), half tone symbol placed in top left corner (-4).
- `⿱B1Kh4+3` → Combined character consisting of `B1` on top of `Kh4+3`.

## Examples
See [`examples/`](examples) for SVG renderings.

## Usage
- Markdown / Blog: QATT code as text, sign rendered as SVG  
- Referenceable for scientific publications
