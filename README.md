# MINMULMAX

WAP to create three input boxes and name it as Min, Max and Mul respectively with one Button named  as "Validate".

Requirement
1. Create three input boxes with labels : a.Min (minimum)   b.Max (maximum)   c.Mul (Multiplier)
2. Create a button and name it as "Validate".
3. Following conditions should get satisfied :
   *Mandatory condition :  Mul should alway be a factor of Min & Max
                           i.e. Min & Max should always be divisible by Mul.
                           If only Max is divisible & Min is not divisible, mark the latter one as red and vice-versa.
                           else mark the input box red for whichever value is wrong(Min/ Max).
   
   Secondary conditions :a) Min < Max
                         b) Mul < Max .
                         c) Mul can be less than or eaqaul to Min i.e.  Mul<=Min .

4: If any conditions gets false, then that box should be highlighted by making the border of that box as "red".

A .  Mul should be the factor of Min & Max.
      min/mul => remainder=0  ------------> false - mark as red   
      OR  max/mul => reaminder=0 ------------> false - mark as red
      If both are not divisile by Mul , mark Mul as red

B.  Min < Max  ------------> false - mark Min as red

C.  Mul < Max  ------------> false - mark Mul as red

D. Mul <= Min------------> false - mark Mul as red


MIN   MAX    MUL     Test Conditions
 2.5   5     2.5    All Conditions are true
-2     4.1   2      A - false (Max is not divisible by Mul)
-2     4    -2      All Conditions are true
-100   100   1      A - true, B - true , C -true, D- false(Mul is not less than min)
-50     50   0      A - false (Mul is not a factor of Max/Min)
100    100   -50    All Conditions are true
6      6.8   3.4    A - false (Min is not divisible by Mul)
6      12     6     All Conditions are true
A       B     C     Incorrect Input  
100    50     25    A - true, B - false (Min is not less than Max)
50      125   25    All Conditions are true
50      101   25    A - false(Max is not divisible by Mul)
25      50     0    A - false (Mul is not a factor of Max/Min)






D. Mul <= Min------------> false - mark Mul as redD. Mul <= Min------------> false - mark Mul as red
