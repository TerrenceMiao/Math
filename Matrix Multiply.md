Linear Transformation / Matrix Multiply
---------------------------------------

The input embedding vector:

$$
\left(\begin{array}{cc}
0\\
1\\
0\\
0
\end{array}\right)
$$

is multiplied by the weight matrix **W**:

$$
\left(\begin{array}{cc}
1 & 1 & 0 & 0\\
0 & 1 & 0 & 1\\
1 & 0 & 1 & 0\\
1 & -1 & 0 & 0
\end{array}\right)
$$

like:


$$
\left(\begin{array}{cc}
1 & 1 & 0 & 0\\
0 & 1 & 0 & 1\\
1 & 0 & 1 & 0\\
1 & -1 & 0 & 0
\end{array}\right)
\left(\begin{array}{cc}
0\\
1\\
0\\
0
\end{array}\right)
$$

and then added with the bias vector **b**:

$$
\left(\begin{array}{cc}
0\\
0\\
-1\\
0
\end{array}\right)
$$

The formula is:

```
[ 1*0 + 1*1 + 0*0 + 0*0 ] + 0 = 1

[ 0*0 + 1*1 + 0*0 + 1*0 ] + 0 = 1

[ 1*0 + 0*1 + 1*0 + 0*0 ] + (-1) = -1

[ 1*0 + (-1)*1 + 0*0 + 0*0] + 0 = -1
```

$$
\left(\begin{array}{cc}
1\\
1\\
-1\\
-1
\end{array}\right)
$$