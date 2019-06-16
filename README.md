# RSA-Python
The RSA algorithm coded in Python

Created in collaboration with [Unnikrishnan Menon](https://github.com/7enTropy7)

**RSA Algorithm**
* Pick two large primes <a href="https://www.codecogs.com/eqnedit.php?latex=p,q" target="_blank"><img src="https://latex.codecogs.com/gif.latex?p,q" title="p,q" /></a>
* Compute <a href="https://www.codecogs.com/eqnedit.php?latex=n=pq" target="_blank"><img src="https://latex.codecogs.com/gif.latex?n=pq" title="n=pq" /></a> and <a href="https://www.codecogs.com/eqnedit.php?latex=\phi(n)=(p-1)(q-1)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\phi(n)=(p-1)(q-1)" title="\phi(n)=(p-1)(q-1)" /></a>
* Choose a public key <a href="https://www.codecogs.com/eqnedit.php?latex=e" target="_blank"><img src="https://latex.codecogs.com/gif.latex?e" title="e" /></a> such that <a href="https://www.codecogs.com/eqnedit.php?latex=1<e<\phi(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?1<e<\phi(n)" title="1<e<\phi(n)" /></a> and <a href="https://www.codecogs.com/eqnedit.php?latex=\text{gcd}(e,\phi(n))=1" target="_blank"><img src="https://latex.codecogs.com/gif.latex?\text{gcd}(e,\phi(n))=1" title="\text{gcd}(e,\phi(n))=1" /></a>
* Calculate <a href="https://www.codecogs.com/eqnedit.php?latex=d" target="_blank"><img src="https://latex.codecogs.com/gif.latex?d" title="d" /></a> such that <a href="https://www.codecogs.com/eqnedit.php?latex=de\equiv1\mod&space;\phi(n)" target="_blank"><img src="https://latex.codecogs.com/gif.latex?de\equiv1\mod&space;\phi(n)" title="de\equiv1\mod \phi(n)" /></a>
* Let the message **key** be <a href="https://www.codecogs.com/eqnedit.php?latex=m" target="_blank"><img src="https://latex.codecogs.com/gif.latex?m" title="m" /></a>
* **Encrypt: **<a href="https://www.codecogs.com/eqnedit.php?latex=c\equiv&space;m^e\mod&space;n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?c\equiv&space;m^e\mod&space;n" title="c\equiv m^e\mod n" /></a>
* **Decrypt: **<a href="https://www.codecogs.com/eqnedit.php?latex=m\equiv&space;c^d\mod&space;n" target="_blank"><img src="https://latex.codecogs.com/gif.latex?m\equiv&space;c^d\mod&space;n" title="m\equiv c^d\mod n" /></a>

![image](https://user-images.githubusercontent.com/7680591/59566357-3a722d00-902d-11e9-991c-b67e5f369722.png)

And this is what a code says….
![rsa](https://user-images.githubusercontent.com/7680591/59566011-0e07e200-9028-11e9-9f54-449d0ff23a28.jpg)

Note that you may have to setup an external dependency environment in some cases, it would create a big chunk of files that are not here due to exceeding the maximum number of files to upload.
