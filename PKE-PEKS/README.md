# PKE-PEKS
<p> 
University of Campinas <br>
Institute of Computing <br>
Laboratory of Security and Applied Cryptography (LASCA) <br>
</p>

<p>
Author: Jheyne N. Ortiz <br/>
Advisors: Ricardo Dahab and Diego F. Aranha <br/>
</p>

<p>
This implementation is intended to have three main C++ classes: HIBE, OT, and PKE-PEKS. Different from Chen and Lin, we replace the HIBE system of Agrawal et al. by the HIBE construction of (Mochetti, and Dahab, 2014) using ideal lattices in order to reduce the public key size.
</p>

<p>
So far, we are considering only the HIBE class, which has four main algorithms: SetUp, KeyDerive, Encrypt, and Decrypt. The SetUp algorithm is already able to generate the system master keys, e.g. two basis for an orthogonal lattice, and it uses the IdealTrapGen algorithm (Stehlé et al., 2009).
</p>

<p>
In focus, we have the KeyDerive algorithm that requires samples from a discrete Gaussian distribution. This project includes the (on going) constant-time implementation of both Ziggurat (Buchmann et al., 2014) and Knuth-Yao (Roy, Vercauteren, and Verbauwhede, 2013) sampling algorithms. 
</p>