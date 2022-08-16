## Index
![dark](https://user-images.githubusercontent.com/12748752/132402918-976c6cc7-cc94-4267-9513-b3937504eb63.png)

## Linear Combinations, Span, Linear Independence
![dark](https://user-images.githubusercontent.com/12748752/132402918-976c6cc7-cc94-4267-9513-b3937504eb63.png)
Lets see at three fundamental ideas in linear algebra, the idea of **Linear combinations**, **Span** and **Linear independence**.

### Linear Combinations
![light](https://user-images.githubusercontent.com/12748752/132402912-1a2a215e-de2f-4536-b28e-e75197136af9.png)
A linear combination of the set of vectors <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{&space;\{v^{(1)},\cdots,v^{(n)}\}}}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{ \{v^{(1)},\cdots,v^{(n)}\}}}" align="center"/> is given by multiplying each vector by a corresponding scalar coefficient and adding the results.

<img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{\sum_{\textit{i}}\alpha_\textit{i}&space;v^{(\textit{i})}}}\&space;\&space;&space;{\color{Blue}\mathbf{&space;=&space;\alpha_\textit{1}&space;v^{(\textit{1})}&space;&plus;\alpha_\textit{2}&space;v^{(\textit{2})}&space;&plus;\cdots&plus;\alpha_\textit{n}&space;v^{(\textit{n})}&space;}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{\sum_{\textit{i}}\alpha_\textit{i} v^{(\textit{i})}}}\ \ {\color{Blue}\mathbf{ = \alpha_\textit{1} v^{(\textit{1})} +\alpha_\textit{2} v^{(\textit{2})} +\cdots+\alpha_\textit{n} v^{(\textit{n})} } }" align="center"/>

#### Example : <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v_{1}=&space;\begin{bmatrix}1&space;\\2&space;\\3\end{bmatrix},&space;v_{2}=&space;\begin{bmatrix}2&space;\\0&space;\\3\end{bmatrix}}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v_{1}= \begin{bmatrix}1 \\2 \\3\end{bmatrix}, v_{2}= \begin{bmatrix}2 \\0 \\3\end{bmatrix}}" align="center"/>

<img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v_{3}=&space;v_{1}&space;&plus;&space;2v_{2}=&space;\begin{bmatrix}5&space;\\2&space;\\9\end{bmatrix}}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v_{3}= v_{1} + 2v_{2}= \begin{bmatrix}5 \\2 \\9\end{bmatrix}}" align="center"/>

#### Note: <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v_{3}=&space;[v_{1}&space;&space;v_{2}]\begin{bmatrix}1&space;\\&space;2&space;\end{bmatrix}&space;=&space;\begin{bmatrix}1&space;&&space;2&space;\\2&space;&&space;0\\3&3\end{bmatrix}\begin{bmatrix}1&space;\\&space;2&space;\end{bmatrix}}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v_{3}= [v_{1} v_{2}]\begin{bmatrix}1 \\ 2 \end{bmatrix} = \begin{bmatrix}1 & 2 \\2 & 0\\3&3\end{bmatrix}\begin{bmatrix}1 \\ 2 \end{bmatrix}}" align="center"/>

#### Matrix multiplications can be interpreted in terms of linear combinations of columns

* <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v&space;=}\begin{bmatrix}1&space;&&space;2&space;\\2&space;&&space;0\\3&3\\\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{v =}\begin{bmatrix}1 & 2 \\2 & 0\\3&3\\\end{bmatrix} }" align="center"/>
* <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{A&space;=}\begin{bmatrix}1&space;&&space;3&space;\\2&space;&&space;4\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{A =}\begin{bmatrix}1 & 3 \\2 & 4\end{bmatrix} }" align="center"/>
* If **V * A** 
<img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{V&space;*&space;A&space;=}\begin{bmatrix}5&space;&&space;11&space;\\2&space;&&space;6\\9&space;&&space;21\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{V * A =}\begin{bmatrix}5 & 11 \\2 & 6\\9 & 21\end{bmatrix} }" />

* Here the first column <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\begin{bmatrix}{\color{Blue}5}&space;\\{\color{Blue}2}\\{\color{Blue}9}\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\begin{bmatrix}{\color{Blue}5} \\{\color{Blue}2}\\{\color{Blue}9}\end{bmatrix} }" align="center"/> looks similar coz the same thing happed here as that of in case of vector.
* Lets think two columns as two vectors like <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{V&space;=}\begin{bmatrix}{\color{Blue}&space;\overrightarrow{\mathbf{v_1&space;}}}&{\color{Blue}\overrightarrow{\mathbf{v_2}&space;}&space;}\\1&space;&&space;2&space;\\2&space;&&space;0\\3&3\\\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{V =}\begin{bmatrix}{\color{Blue} \overrightarrow{\mathbf{v_1 }}}&{\color{Blue}\overrightarrow{\mathbf{v_2} } }\\1 & 2 \\2 & 0\\3&3\\\end{bmatrix} }" align="center"/> and this first column <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{A&space;=}\begin{bmatrix}{\color{Blue}&space;1}&space;&&space;3&space;\\{\color{Blue}&space;2}&space;&&space;4\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{A =}\begin{bmatrix}{\color{Blue} 1} & 3 \\{\color{Blue} 2} & 4\end{bmatrix} }" align="center"/> as the preveous section vector solutions.

* So the first column calculation is like <img src="https://latex.codecogs.com/svg.image?{\color{Purple}&space;{\color{Blue}&space;1}&space;\times&space;\overrightarrow{\mathbf{v_1}}&space;&plus;&space;{\color{Blue}&space;2}&space;\times&space;\overrightarrow{\mathbf{v_2}}=&space;\begin{bmatrix}5&space;\\2&space;\\9\end{bmatrix}}&space;&space;" title="https://latex.codecogs.com/svg.image?{\color{Purple} {\color{Blue} 1} \times \overrightarrow{\mathbf{v_1}} + {\color{Blue} 2} \times \overrightarrow{\mathbf{v_2}}= \begin{bmatrix}5 \\2 \\9\end{bmatrix}} " align="center" />
* Similarly for the second column <img src="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{A&space;=}\begin{bmatrix}1&space;&&space;{\color{Blue}&space;3}&space;\\2&space;&{\color{Blue}&space;4}\end{bmatrix}&space;}" title="https://latex.codecogs.com/svg.image?{\color{Purple}\mathbf{A =}\begin{bmatrix}1 & {\color{Blue} 3} \\2 &{\color{Blue} 4}\end{bmatrix} }" align="center"/> 
* <img src="https://latex.codecogs.com/svg.image?{\color{Purple}&space;{\color{Blue}&space;3&space;}&space;&space;\mathbf{v_1}&space;&plus;&space;{\color{Blue}&space;4}&space;\mathbf{v_2}=&space;\begin{bmatrix}11&space;\\6&space;\\21\end{bmatrix}}&space;" title="https://latex.codecogs.com/svg.image?{\color{Purple} {\color{Blue} 3 } \mathbf{v_1} + {\color{Blue} 4} \mathbf{v_2}= \begin{bmatrix}11 \\6 \\21\end{bmatrix}} " align="center"/>