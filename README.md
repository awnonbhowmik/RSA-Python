# RSA-Python
The RSA algorithm coded in Python

Created in collaboration with [Unnikrishnan Menon](https://github.com/7enTropy7)

**RSA Algorithm**
* Pick two large primes $p,q$.
* Compute $n=pq$ and $\varphi(n)=\mathrm{lcm}(p-1,q-1)$
* Choose a public key $e$ such that $1<e<\varphi(n)$ and $\gcd(e,\varphi(n))=1$
* Calculate $d$ such that $de\equiv 1 \pmod\varphi(n)$
* Let the message **key** be $m$
* **Encrypt: ** $c\equiv m^e\pmod n$
* **Decrypt: ** $m\equiv c^d\pmod n$

![image](https://user-images.githubusercontent.com/7680591/59566357-3a722d00-902d-11e9-991c-b67e5f369722.png)

And this is what a code says….
![rsa](https://user-images.githubusercontent.com/7680591/59566011-0e07e200-9028-11e9-9f54-449d0ff23a28.jpg)

Note that you may have to setup an external dependency environment in some cases, it would create a big chunk of files that are not here due to exceeding the maximum number of files to upload.
