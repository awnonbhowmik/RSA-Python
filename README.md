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

<math xmlns="http://www.w3.org/1998/Math/MathML" display="block">
  <mtable displaystyle="true">
    <mlabeledtr>
      <mtd id="mjx-eqn-_3" />
      <mtd>
        <mtable columnalign="center center" rowspacing="4pt" columnspacing="1em" rowlines="solid solid none none none none solid none solid none none solid none solid" columnlines="solid" frame="solid">
          <mtr>
            <mtd>
              <mtext>Message</mtext>
            </mtd>
            <mtd>
              <mtext>H</mtext>
            </mtd>
            <mtd>
              <mtext>e</mtext>
            </mtd>
            <mtd>
              <mtext>l</mtext>
            </mtd>
            <mtd>
              <mtext>l</mtext>
            </mtd>
            <mtd>
              <mtext>o</mtext>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mtext>ASCII Code</mtext>
            </mtd>
            <mtd>
              <mn>72</mn>
            </mtd>
            <mtd>
              <mn>101</mn>
            </mtd>
            <mtd>
              <mn>108</mn>
            </mtd>
            <mtd>
              <mn>108</mn>
            </mtd>
            <mtd>
              <mn>111</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>p</mi>
              <mo>=</mo>
              <mn>11</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>q</mi>
              <mo>=</mo>
              <mn>13</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>n</mi>
              <mo>=</mo>
              <mn>143</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>&#x03D5;<!-- ϕ --></mi>
              <mo stretchy="false">(</mo>
              <mi>n</mi>
              <mo stretchy="false">)</mo>
              <mo>=</mo>
              <mn>120</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>e</mi>
              <mo>=</mo>
              <mn>77</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mtext>Encryption</mtext>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>c</mi>
              <mo>&#x2261;<!-- ≡ --></mo>
              <msup>
                <mi>m</mi>
                <mi>e</mi>
              </msup>
              <mspace width="0.667em" />
              <mi>mod</mi>
              <mspace width="thinmathspace" />
              <mspace width="thinmathspace" />
              <mi>n</mi>
            </mtd>
            <mtd>
              <mn>63</mn>
            </mtd>
            <mtd>
              <mn>95</mn>
            </mtd>
            <mtd>
              <mn>114</mn>
            </mtd>
            <mtd>
              <mn>114</mn>
            </mtd>
            <mtd>
              <mn>89</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>d</mi>
              <mi>e</mi>
              <mo>&#x2261;<!-- ≡ --></mo>
              <mn>1</mn>
              <mspace width="0.667em" />
              <mi>mod</mi>
              <mspace width="thinmathspace" />
              <mspace width="thinmathspace" />
              <mi>&#x03D5;<!-- ϕ --></mi>
              <mo stretchy="false">(</mo>
              <mi>n</mi>
              <mo stretchy="false">)</mo>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mn>77</mn>
              <mi>d</mi>
              <mo>&#x2261;<!-- ≡ --></mo>
              <mn>1</mn>
              <mspace width="0.667em" />
              <mi>mod</mi>
              <mspace width="thinmathspace" />
              <mspace width="thinmathspace" />
              <mn>120</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>d</mi>
              <mo>&#x2261;<!-- ≡ --></mo>
              <mn>53</mn>
              <mspace width="0.667em" />
              <mi>mod</mi>
              <mspace width="thinmathspace" />
              <mspace width="thinmathspace" />
              <mn>120</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mtext>Decrypted ASCII</mtext>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mi>m</mi>
              <mo>&#x2261;<!-- ≡ --></mo>
              <msup>
                <mi>c</mi>
                <mi>d</mi>
              </msup>
              <mspace width="0.667em" />
              <mi>mod</mi>
              <mspace width="thinmathspace" />
              <mspace width="thinmathspace" />
              <mi>n</mi>
            </mtd>
            <mtd>
              <mn>72</mn>
            </mtd>
            <mtd>
              <mn>101</mn>
            </mtd>
            <mtd>
              <mn>108</mn>
            </mtd>
            <mtd>
              <mn>108</mn>
            </mtd>
            <mtd>
              <mn>111</mn>
            </mtd>
          </mtr>
          <mtr>
            <mtd>
              <mtext>Decrypted Message</mtext>
            </mtd>
            <mtd>
              <mtext>H</mtext>
            </mtd>
            <mtd>
              <mtext>e</mtext>
            </mtd>
            <mtd>
              <mtext>l</mtext>
            </mtd>
            <mtd>
              <mtext>l</mtext>
            </mtd>
            <mtd>
              <mtext>o</mtext>
            </mtd>
          </mtr>
        </mtable>
      </mtd>
    </mlabeledtr>
  </mtable>
</math>
And this is what a code says….
![rsa](https://user-images.githubusercontent.com/7680591/59566011-0e07e200-9028-11e9-9f54-449d0ff23a28.jpg)
