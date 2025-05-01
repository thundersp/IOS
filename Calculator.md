## Calculator 
 Steps:
1. Select vertical stack view and add 4 constraints - 0 0 0 0 from the bottom left column
2. Add 2 views from the library into the stack view, hold control and click and drag the bottom view to safe area, choose the option "Equal heights"
3. When you add constraints, it generates a constraints folder, in that, choose the "View.Height" and in the attribute inspector, in the right panel, add multiplier as 0.66
4. Add label in the top view as 0
5. Add Vertical stack view in the bottom view, add constraints as 0 0 0 0, in the right panel, select distribution as Fill equally and spacing as 1
6. Add horizontal stack to the above vertical stack, and apply distribution and spacing as above
7. In that Horizontal stack, add a button with gray bg, and copy paste 3 times, then copy paste the parent horizontal stack 4 times.
8. In the last row, delete one button, Hold control from the left button and relase to middle, then middle to right. Choose the equal widths option. 
9. After choosing equal widths, it will form a constraints folder in the bottom stack, in the first entry, in the attribute inspector, in the "Multiplier" enter "2".
10. In the parent stack, that is the horizontal stack in which the three buttons are there, in the right panel, In distribution, choose fill proportionally
