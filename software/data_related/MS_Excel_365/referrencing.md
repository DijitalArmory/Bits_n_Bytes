# Absolute & Relative Referrencing

In Excel, relative and absolute referencing are two methods used to refer to cells in formulas. These referencing methods affect how formulas behave when copied or filled to other cells.


## Relative Referencing
Relative referencing is the __default__ referencing method in Excel. When you create a formula using relative referencing, the cell references are adjusted automatically based on their relative position when the formula is copied or filled to other cells.
For example, if you have a formula in cell B2 that references cell A1, and you copy the formula to cell B3, the formula will adjust to reference cell A2. The formula in B3 will maintain the same relative position as the formula in B2.

## Absolute Referencing
Absolute referencing is used when you want to _lock_ a specific cell reference in a formula, preventing it from adjusting when the formula is copied or filled to other cells. This is useful when you want a certain cell reference to remain constant regardless of where the formula is copied.
To create an absolute reference, you use the dollar sign ($) before the column letter, row number, or both. The dollar sign makes that part of the reference absolute.

For example, if you have a formula in cell B2 that references cell `$A$1`, and you copy the formula to cell B3, the formula will still reference cell `$A$1`, maintaining the same absolute reference.

## Mixed Referencing
Mixed referencing is a combination of relative and absolute referencing. You can make either the column reference or the row reference absolute, while leaving the other part as relative.
For example, if you have a formula in cell B2 that references cell $A1, and you copy the formula to cell C2, the column reference will stay fixed as $A, but the row reference will adjust to C1. If you copy the formula to cell B3, both the column and row references will adjust accordingly.

The choice between relative and absolute referencing depends on the specific requirements of your calculations. Relative referencing is often used when you want formulas to automatically adjust based on the relative position of the cells. Absolute referencing is useful when you want to lock a specific reference that should not change when the formula is copied. Mixed referencing provides flexibility by allowing certain parts of the reference to be fixed while others adjust.

---
---
---

### Keyboard Shortcut
* click on cell
* select __F4__

---
---
---

* [Example Video](https://www.youtube.com/watch?v=fODnNDNMXiI&list=WL&index=89&t=9934s)
* __Example__: To Sum the cells of column B to the cell F1, absolutley reference F1
* `=SUM(B2*$F1)`
* drage from B2 down the column to apply to the rest of the column