# RSA-Python
The RSA algorithm coded in Python

**RSA Algorithm**
* Pick two large primes $p,q$
* Compute $n=pq$ and $\phi(n)=(p-1)(q-1)$
* Choose a public key $e$ such that $1<e<\phi(n)$ and $\text{gcd}(e,\phi(n))=1$
* Calculate $d$ such that $de\equiv 1\mod\phi(n)$
* Let the message **key** be $m$
* **Encrypt: **$c\equiv m^e\mod n$
* **Decrypt: **$m\equiv c^d\mod n$

$\begin{array}{|c|c|}\hline\text{Message}&\text{H}&\text{e}&\text{l}&\text{l}&\text{o}\\\hline\text{ASCII Code}&72&101&108&108&111\\\hline p=11\\q=13\\n=143\\\phi(n)=120\\e=77\\\hline \text{Encryption}\\c\equiv m^e\mod n&63&95&114&114&89\\\hline de\equiv 1\mod \phi(n)\\77d\equiv1\mod 120\\d\equiv53\mod120\\\hline\text{Decrypted ASCII}\\m\equiv c^d\mod n&72&101&108&108&111\\\hline\text{Decrypted Message}&\text{H}&\text{e}&\text{l}&\text{l}&\text{o}\\\hline\end{array}\tag*{}$
And this is what a code says….
![rsa](https://user-images.githubusercontent.com/7680591/59566011-0e07e200-9028-11e9-9f54-449d0ff23a28.jpg)
