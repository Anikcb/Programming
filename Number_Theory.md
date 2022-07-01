<h1 align="center">Number Theory</h1>

## Binary Exponentiation <sup>[[1]](https://cp-algorithms.com/algebra/binary-exp.html)</sup><sup>[[2]](https://cs.stackexchange.com/questions/77016/modular-multiplication)</sup>
<pre>
      - Binary Exponentiation[1]
      - modular multiplication[2]
</pre>
### Problems

<details>
  <summary> LASTDIG - SPOJ </summary>

  <blockquote>
  

  ```sh
  https://www.spoj.com/problems/LASTDIG/
  ```
     
        
<details>

  <summary>Solutions</summary>
  

  <details><summary> Solution-1 </summary>
  <blockquote>

  ```c++
      #include<iostream>
      using namespace std;


      #define          ll     long long int
      void FLASH() {ios_base::sync_with_stdio(false); cin.tie(NULL); cout.tie(NULL);}


      ll bigmod ( ll a, ll p, ll m )
      {
          ll res = 1;
          ll x = a%m;
          if(x==0)return 0;

          while ( p )
          {
              if ( p & 1 )
              {
                  res = ( res * x ) % m;
              }
              x = ( x * x ) % m;
              p = p >> 1;
          }

          return res;
      }

      int main()
      {
           FLASH();
           ll t;
           cin>>t;
           while(t--)
           {
               ll a,b;
               cin>>a>>b;
               cout<<bigmod(a,b,10)<<endl;
           }



          return 0;
      }

  ```
  
  </blockquote>
  </details>
  </details>
</details>
       
        
        
<details>
  <summary> LOCKER - SPOJ </summary>

  <blockquote>

  ```sh
  https://www.spoj.com/problems/LOCKER/
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  https://palak001.medium.com/spoj-locker-magic-of-the-locker-a758bccf432f
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>
      
      
      
      
      
<details>
  <summary> ZSUM - SPOJ </summary>

  <blockquote>
  

  ```sh
 https://www.spoj.com/problems/ZSUM/
  ```
     
        
<details>

  <summary>Solutions</summary>
  

  <details><summary> Solution-1 </summary>
  <blockquote>

  ```c++
      
      #include <iomanip>
      #include <iostream>
      #include <algorithm>
      #include <cstdio>
      #include <cstdlib>
      #include <cstring>
      #include <string>
      #include <cmath>
      #include <vector>
      #include <set>
      #include <map>
      #include <unordered_set>
      #include <unordered_map>
      #include <stack>
      #include <queue>
      #include <deque>
      #include <iterator>
      #include <bitset>
      #include <assert.h>
      #include <new>
      #include <sstream>
      #include <time.h>


      using namespace std;
      typedef long long ll;
      #define     re                return
      #define     IOS               ios_base::sync_with_stdio(false); cin.tie(NULL); cout.tie(NULL);




      ll bigmod(ll a,ll p,ll m)
      {
          ll x=a%m,res=1;
          if(x==0)re 0;
          while(p){
              if(p&1)res = (res*x)%m;
              x = (x*x)%m;
              p>>=1;
          }
          re res;
      }


      int main()
      {
          IOS;
          ll tst=1;
          //cin>>tst;
          for(ll tt=1;  ;tt++)
          {
              //code
              ll n,k;
              cin>>n>>k;
              if(!n && !k)break;
              ll val=(2*bigmod(n-1,k,MOD))%MOD + bigmod(n,k,MOD) + (2*bigmod(n-1,n-1,MOD))%MOD + bigmod(n,n,MOD);
              cout<<val%MOD<<endl;

          }


          return 0;
      }


  ```
  
  </blockquote>
  </details>
  </details>
</details><br>      
      
## Modular Inverse <sup>[[1]](https://forthright48.com/modular-multiplicative-inverse/?fbclid=IwAR0GqrqHtTnIuSGQ1ii8lqELD9f8mqc0tJPhpJM7L6ufe5IlpndQt6jHqYo)</sup><sup>[[2]](https://www.youtube.com/watch?v=mgvA3z-vOzc&t=61s&ab_channel=RandellHeyman)</sup><sup>[[3]](https://www.youtube.com/watch?v=shaQZg8bqUM&t=8s&ab_channel=LearnMathTutorials)</sup><sup>[[4]](https://cp-algorithms.com/algebra/module-inverse.html)</sup>
<pre>
      - Modular Multiplicative Inverse - forthright48[1]
      - Modular inverse made easy[2]
      - How To Find The Inverse of a Number[3]
      - Modular Multiplicative Inverse - Cp Algorithm[4]
</pre> 
### Problems
<details>
  <summary> LOCKER - SPOJ </summary>

  <blockquote>

  ```sh
  https://www.spoj.com/problems/LOCKER/
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  https://palak001.medium.com/spoj-locker-magic-of-the-locker-a758bccf432f
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details><br>  
        
        
 
        
        
        
        
## Sieve of Eratosthenes <sup>[[1]](https://forthright48.com/sieve-of-eratosthenes-generating-primes/)</sup><sup>[[2]](https://cp-algorithms.com/algebra/sieve-of-eratosthenes.html)</sup><sup>[[3]](https://forthright48.com/segmented-sieve-of-eratosthenes)</sup>
<pre>
      - Sieve of Eratosthenes - forthright48[1]
      - Sieve of Eratosthenes - Cp Algorithm[2]
      - Segmented Sieve of Eratosthenes -  forthright48[3]
</pre> 
### Problems
<details>
  <summary> TDPRIMES - SPOJ </summary>

  <blockquote>

  ```sh
  https://www.spoj.com/problems/TDPRIMES/
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  https://ideone.com/k3Ykm0
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details><br>  
        
        
        
        
        
        
        
        
        
        
## Euclidean Algorithm <sup>[[1]](https://youtu.be/H_2_nqKAZ5w)</sup><sup>[[2]](https://www.freecodecamp.org/news/euclidian-gcd-algorithm-greatest-common-divisor/)</sup>
<pre>
      - Euclidean Algorithm(Proof) - Youtube[1]
      - Euclidian Algorithm - FreeCodeCamp[2]
</pre> 
### Problems
<details>
  <summary>11827 - Maximum GCD </summary>

  <blockquote>

  ```sh
  https://onlinejudge.org/index.php?option=onlinejudge&Itemid=8&page=show_problem&problem=2927
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  Solve it!!
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details><br>          
        
        

        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
## Extend Euclidean Algorithm <sup>[[1]](https://youtu.be/hB34-GSDT3k)</sup><sup>[[2]](https://www.youtube.com/watch?v=fz1vxq5ts5I&t=47s&ab_channel=EmilyS)</sup><sup>[[3]](https://returnzerooo.wordpress.com/2017/08/12/%E0%A6%8F%E0%A6%95%E0%A7%8D%E0%A6%B8%E0%A6%9F%E0%A7%87%E0%A6%A8%E0%A7%8D%E0%A6%A1%E0%A7%87%E0%A6%A1-%E0%A6%87%E0%A6%89%E0%A6%95%E0%A7%8D%E0%A6%B2%E0%A6%BF%E0%A6%A1%E0%A7%80%E0%A7%9F%E0%A6%BE%E0%A6%A8/)</sup><sup>[[4]](https://forthright48.com/extended-euclidean-algorithm/)</sup><sup>[[5]](https://forthright48.com/linear-diophantine-equation/)</sup><sup>[[6]](https://cp-algorithms.com/algebra/extended-euclid-algorithm.html)</sup><sup>[[7]](https://cp-algorithms.com/algebra/linear-diophantine-equation.html)</sup>
<pre>
      - The Extended Euclidean algorithm - Youtube[1]
      - Extended Euclidean Algorithm and Inverse Modulo - FreeCodeCamp[2]
      - এক্সটেন্ডেড ইউক্লিডীয়ান অ্যালগোরিদম - Return 0[3]
      - Extended Euclidean Algorithm - forthright48[4]
      - Linear Diophantine Equation  - forthright48[5]
      - Extended Euclidean Algorithm - Cp Algorithm[6]
      - Linear Diophantine Equation - Cp Algorithm[7]
</pre> 
### Problems
<details>
  <summary> Extended Euclidean Algorithm applications</summary>

  <blockquote>

  ```sh
  https://codeforces.com/blog/entry/10575?locale=en
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  Solve them!!
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details><br>           
        
        
        
        
        
        
        
        
        
        
        
        
        
## Chicken McNugget Theorem <sup>[[1]](https://www.youtube.com/watch?v=SLyVAR3JV5A)</sup><sup>[[2]](https://www.youtube.com/watch?v=VUKTtptZpQs&ab_channel=ELITESGRID-CATPREP)</sup><sup>[[3]](https://www.cantorsparadise.com/chicken-mcnugget-theorem-1df48d273a57)</sup>
<pre>
      - Frobenius Coin Problem (Chicken McNugget Theorem) - Youtube[1]
      - Number System Concept 4 ( Chicken Mcnugget Theorem) - Youtube[2]
      - Chicken McNugget Theorem - Medium[3]
</pre> 
### Problems
<details>
  <summary>Get AC in one go - CodeChef</summary>

  <blockquote>

  ```sh
  https://www.codechef.com/problems/COPR16G
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  https://www.codechef.com/viewsolution/63102204
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>  <br>  
        
        
        
        
        
        
        
        
        
        
        
        
        
        
## Binomial Coefficients <sup>[[1]](https://www.youtube.com/watch?v=o-ZtGGXLogE&ab_channel=CodeWhoop)</sup><sup>[[2]](https://cp-algorithms.com/combinatorics/binomial-coefficients.html)</sup>
<pre>
      - Binomial Coefficient using C++ - Youtube[1]
      - Binomial Coefficients - Cp Algorithm[2]
</pre> 
### Problems
<details>
  <summary>Get AC in one go - CodeChef</summary>

  <blockquote>

  ```sh
  https://www.codechef.com/problems/COPR16G
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  https://www.codechef.com/viewsolution/63102204
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details><br>   
        
        
        
        
        
        
        
## Sieve of Eratosthenes <sup>[[1]](https://forthright48.com/sieve-of-eratosthenes-generating-primes/)</sup><sup>[[2]](https://cp-algorithms.com/algebra/sieve-of-eratosthenes.html)</sup><sup>[[3]](https://forthright48.com/segmented-sieve-of-eratosthenes)</sup>
<pre>
      - Sieve of Eratosthenes, Generating Primes - forthright48[1]
      - Binomial Coefficients - Cp Algorithm[2]
      - Segmented Sieve of Eratosthenes - forthright48[3]
</pre> 
### Problems
<details>
  <summary>Get AC in one go - CodeChef</summary>

  <blockquote>

  ```sh
  https://www.codechef.com/problems/COPR16G
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
  https://www.codechef.com/viewsolution/63102204
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details><br><br>   
        
