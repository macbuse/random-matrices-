# Simpler integer matrices

One of the annoying things when teaching is that 
the **smartass** that sets the questions will just
take random integer coefficients without thinking
so you get a matrix that isn't nice to work with.


This notebook attempts to solve the problem of the poor instructor/grader.

- 3x3 rank 2 matrix with kernel and equation $ax + by + cz = 0$ for the image
- 3x3 invertible matrix with given determinant and hints on how to find its inverse
- a function for rendering an np.array as a LaTex pmatrix

---

## what you get?

def rand_rank2(max_int=6):<br>

    ''' returns 
        A rank 2,  3x3 matrix
        K vector basis for the kernel
        V vector orthogonal to the image
    '''

def rand_inv(high=3,<br>
             D=[1,1,1])->np.array:<br>
    
    ''' returns an invertible matrix with
        - integer coefficients in the range [-high, high] 
        - determinant is the product of the elements of D
        - a list of row operations to put it in upper triangular form
        
        see https://en.wikipedia.org/wiki/Bruhat_decomposition
        
    

---

Copyright 2022  Greg McShane (macbuse.github)

Permission is hereby granted, free of charge, to any person obtaining a copy of this software and associated documentation files (the "Software"), to deal in the Software without restriction, including without limitation the rights to use, copy, modify, merge, publish, distribute, sublicense, and/or sell copies of the Software, and to permit persons to whom the Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE SOFTWARE.