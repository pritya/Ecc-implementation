
Topic : Implementation of Elliptic curve cryptography

           Language - C++
           Files - main.cpp , FiniteFieldElement.hpp
           Compile - g++ main.cpp

           Run - ./a.out


ECC - Cubic curve in finite field
Finite field element class has an Integer in finite field P and Point class has 
a point(x,y) in finite field. ECC contains vector structure for containing all
points that satisfies equation y^2=x^3+ax+b .

Alice's Key Generation
Select private key a 	 a<n
public key PA 	 PA=a*G;

Bob's Key Generation
Select private key b 	 b<n
public key PB 	 PB = b*G

Secret Key by Alice
K = a * PB
Secret Key by Bob
K = b * PA

Encryption by Alice :-
  C1=KG;
  C2=Pm+K*PB;

Decryption by Bob:-
  Pm=C2- nB C1

