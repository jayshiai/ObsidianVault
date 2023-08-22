In A register

If Higher nibble> 9 or CF = 1 then add 60
If Lower nibble >9 or AC  = 1 then add 06


25H + 35H = 5AH;
here A > 9 in lower nibble. Therefore A + 06 = 10 ( 1 carry over)
5 + 1 = 6
there fore 5A = 60 ( 25 + 35)