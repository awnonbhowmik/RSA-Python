# RSA-Python
The RSA algorithm coded in Python

**RSA Algorithm**
* Pick two large primes <a href="https://www.codecogs.com/eqnedit.php?latex=p,q" target="_blank"><img src="https://latex.codecogs.com/gif.latex?p,q" title="p,q" /></a>
* Compute <a href="https://www.codecogs.com/eqnedit.php?latex=n=pq" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n=pq" title="n=pq" /></a> and <a href="https://www.codecogs.com/eqnedit.php?latex=\phi(n)=(p-1)(q-1)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\phi(n)=(p-1)(q-1)" title="\phi(n)=(p-1)(q-1)" /></a>
* Choose a public key <a href="https://www.codecogs.com/eqnedit.php?latex=e" target="_blank"><img src="https://latex.codecogs.com/gif.latex?e" title="e" /></a> such that <a href="https://www.codecogs.com/eqnedit.php?latex=1<e<\phi(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?1<e<\phi(n)" title="1<e<\phi(n)" /></a> and <a href="https://www.codecogs.com/eqnedit.php?latex=\text{gcd}(e,\phi(n))=1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\text{gcd}(e,\phi(n))=1" title="\text{gcd}(e,\phi(n))=1" /></a>
* Calculate <a href="https://www.codecogs.com/eqnedit.php?latex=d" target="_blank"><img src="https://latex.codecogs.com/gif.latex?d" title="d" /></a> such that <a href="https://www.codecogs.com/eqnedit.php?latex=de\equiv1\mod&space;\phi(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?de\equiv1\mod&space;\phi(n)" title="de\equiv1\mod \phi(n)" /></a>
* Let the message **key** be <a href="https://www.codecogs.com/eqnedit.php?latex=m" target="_blank"><img src="https://latex.codecogs.com/gif.latex?m" title="m" /></a>
* **Encrypt: **<a href="https://www.codecogs.com/eqnedit.php?latex=c\equiv&space;m^e\mod&space;n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?c\equiv&space;m^e\mod&space;n" title="c\equiv m^e\mod n" /></a>
* **Decrypt: **<a href="https://www.codecogs.com/eqnedit.php?latex=m\equiv&space;c^d\mod&space;n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?m\equiv&space;c^d\mod&space;n" title="m\equiv c^d\mod n" /></a>

$\begin{array}{|c|c|}\hline\text{Message}&\text{H}&\text{e}&\text{l}&\text{l}&\text{o}\\\hline\text{ASCII Code}&72&101&108&108&111\\\hline p=11\\q=13\\n=143\\\phi(n)=120\\e=77\\\hline \text{Encryption}\\c\equiv m^e\mod n&63&95&114&114&89\\\hline de\equiv 1\mod \phi(n)\\77d\equiv1\mod 120\\d\equiv53\mod120\\\hline\text{Decrypted ASCII}\\m\equiv c^d\mod n&72&101&108&108&111\\\hline\text{Decrypted Message}&\text{H}&\text{e}&\text{l}&\text{l}&\text{o}\\\hline\end{array}\tag*{}$
And this is what a code says….
![rsa](https://user-images.githubusercontent.com/7680591/59566011-0e07e200-9028-11e9-9f54-449d0ff23a28.jpg)
