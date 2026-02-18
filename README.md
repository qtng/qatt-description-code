## QATT Description Code

This repository defines the **QATT Description Code**, a compact, formal notation for describing the **visual structure** of Quốc Âm Tân Tự characters.

Because Quốc Âm Tân Tự symbols are not currently encoded in Unicode, QATT Description Code provides a standardized way to **reference, analyze, and discuss** these characters in technical and academic contexts.

### Basic concept

A QATT code describes **how a character looks**, not what it means.  
Each code consists of a **base symbol**, optionally followed by **dot markers** and **tone indicators** that specify their visual placement.  
More complex characters can be expressed by **combining multiple QATT codes** using ideographic description sequences (IDS).

**Examples:**

- `Dd5+1` → `⁰壬`  
  Base symbol **Dd**, with a dot placed at the start of the vertical **main stroke** and a full tine symbol in the top left corner.

- `Ch1-4` → `꜆牛`  
  Base symbol **Ch**, with a dot on the top left of the **support rectangle** and a half tone marker in the bottom-left corner.

- `⿱ThDd-2` → `芏꜂`  
  A compound character formed by placing **Th** above **Dd**, with a half tone marker at the top-right.

The complete syntax, component definitions, and formal rules are described in the [Full Specification](SPEC.md).

---

## Mã mô tả QATT

Kho lưu trữ này định nghĩa **Mã mô tả QATT**, một hệ thống ký hiệu ngắn gọn và hình thức nhằm mô tả **cấu trúc trực quan** của các ký hiệu Quốc Âm Tân Tự.

Do các ký hiệu Quốc Âm Tân Tự hiện chưa được mã hóa trong Unicode, mã mô tả QATT cung cấp một phương thức thống nhất để **dẫn chiếu, phân tích và thảo luận** các ký hiệu này trong các ngữ cảnh kỹ thuật và học thuật.

### Khái niệm cơ bản

Một mã QATT mô tả **hình thức biểu hiện của ký hiệu**, không mô tả ý nghĩa ngữ nghĩa.  
Mỗi mã bao gồm một **ký hiệu cơ sở** (cán tự), có thể kèm theo **dấu phẩy** và **thanh điệu** âm/dương để chỉ rõ vị trí hiển thị của chúng.  
Các ký tự phức hợp được biểu diễn bằng cách **kết hợp nhiều mã QATT** thông qua IDS (Ideographic Description Sequence).

**Ví dụ:**

- `Dd5+1` → `⁰壬`  
  Cán tự **Dd**, với dấu phẩy đặt tại đầu **nét chính** với thanh điêu dương ở góc trên bên trái.

- `Ch1-4` → `꜀牛`  
  Cán tự **Ch**, với dấu phẩy ở trên bên trái của hình chữ nhật của **nét phụ** với thanh điệu dương ở góc dưới bên trái.

- `⿱ThDd-2` → `芏꜄`  
  Chữ phức hợp gồm **Th** đặt phía trên **Dd**, với thanh điệu âm ở góc trên bên phải.

Cú pháp đầy đủ, định nghĩa các thành phần và các quy tắc hình thức được trình bày trong [Tài liệu đặc tả đầy đủ QATT-DC](SPEC.md).

# Lookup table - Bảng tra
tbd
