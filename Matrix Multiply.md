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

is multiplied by the weight matrix _**W**_:

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

and then added with the bias vector _**b**_:

$$
\left(\begin{array}{cc}
0\\
0\\
-1\\
0
\end{array}\right)
$$

The formula: _z_ = _Wx_ + _b_, _x_ is word embedding

```
[ 1 x 0 + 1 x 1 + 0 x 0 + 0 x 0 ] + 0 = 1

[ 0 x 0 + 1 x 1 + 0 x 0 + 1 x 0 ] + 0 = 1

[ 1 x 0 + 0 x 1 + 1 x 0 + 0 x 0 ] + (-1) = -1

[ 1 x 0 + (-1) x 1 + 0 x 0 + 0 x 0] + 0 = -1
```

$$
\left(\begin{array}{cc}
1\\
1\\
-1\\
-1
\end{array}\right)
$$