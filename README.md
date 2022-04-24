
# How to Boost your Rating!!🔥🔥

<p align="right"> <a href="https://youtu.be/4Fbd59j_PRI" target="blank"><img width="300" src="https://github.com/Anikcb/Programming/blob/main/Data/oct.gif?raw=true" alt="anik33122906" /><img width="400" src="https://github.com/Anikcb/Programming/blob/main/Data/you_1.png?raw=true" alt="anik33122906" /></a> </p>





# Useful links
```sh
      https://www.youtube.com/channel/UCN_pqF_Y6IObpxapaQPHWZg
```
```sh
      https://blog.shahjalalshohag.com/topic-list/
```
```sh
      https://forthright48.com/p-cpps-101/
```
```sh
     https://github.com/me-shaon/bangla-programming-resources    
```





</br></br>
<h1 align="center">STL</h1>


## Policy Based Data Structure(Ordered_Set) <sup>[[1]](https://youtu.be/MiBrJTNOEP0)</sup><sup>[[2]](https://codeforces.com/blog/entry/11080)</sup><sup>[[3]](https://codeforces.com/blog/entry/13279)</sup>
<pre>
      - Policy Based Data Structure (Bangla) - Youtube[1]
      - C++ STL: Policy based data structures - Codeforces[2]
      - C++ STL: Policy based data structures, Part 2 - Codeforces[3]
</pre> 
### Problems
<details>
  <summary>Stars - Timus</summary>

  <blockquote>

  ```sh
  https://acm.timus.ru/problem.aspx?space=1&num=1028
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```c++
  
     ordered_set s;
     ll n;
     cin>>n;
     for(ll i=1;i<=n;i++)
     {
         ll a,b;
         cin>>a>>b;
         s.insert(make_pair(a,b));
         ll pos=s.order_of_key(make_pair(a,b));
         A[pos]++;
     }
     for(ll i=0;i<n;i++)cout<<A[i]<<endl;
        
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>
  
  
  
  
  
      
      
      
      
      
## Set, Unordered Set, Multiset <sup>[[1]](https://youtu.be/7mx2BasNK0w)</sup><sup>[[2]](https://youtu.be/xelzlR_OGnI)</sup><sup>[[3]](https://www.geeksforgeeks.org/multiset-in-cpp-stl/)</sup>
<pre>
      - SET, UNORDERED SET & MULTISET (Hindi) - Youtube[1]
      - Multiset in C++ STL - Youtube[2]
      - Multiset in C++ - GeeksforGeekss[3]
</pre> 
### Problems
<details>
  <summary>Mahesh and his lost array - CodeChef</summary>

  <blockquote>

  ```sh
     https://www.codechef.com/problems/ANUMLA
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

  </details>      
  
  
  
  
  
  
  
  
  
  
  
  
  ## Priority Queue <sup>[[1]](https://youtu.be/JSqznrzWGvc)</sup><sup>[[2]](https://www.programiz.com/cpp-programming/priority-queue)</sup>
<pre>
      - std::priority_queue In C++ - Youtube[1]
      - C++ Priority Queue - Programiz[2]
</pre> 
### Problems
<details>
  <summary>No Name</summary>

  <blockquote>

  ```sh
     Priority Queue is very useful to solve Graph problems
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
      There is no solution right now!!
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details> 
  
  
  
  
  
  
  
  
  
  
  
  
  
  
  

<h1 align="center">Math</h1>

## Matrix Exponentiation <sup>[[1]](https://youtu.be/EEb6JP3NXBI)</sup><sup>[[2]](https://youtu.be/EEb6JP3NXBI)</sup>
<pre>
      - Solving the Fibonacci Sequence with Matrix Exponentiation[1]
      - What is Fast Exponentiation?[2]
</pre> 
### Problems



<details>
  <summary> SUMMUL - SPOJ </summary>

  <blockquote>
  

  <details><summary> Problem Link </summary>
  <blockquote>

  ```sh
  https://www.spoj.com/problems/SUMMUL/
  ```
  
  </blockquote>
  </details>
  
        
        
<details>

  <summary>Solutions </summary>
  

  <details><summary> Solution-1 </summary>
  <blockquote>

  ```c++
      //#include <ext/pb_ds/assoc_container.hpp>
      //#include <ext/pb_ds/tree_policy.hpp>
      //#include<bits/stdc++.h>
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


      //using    namespace __gnu_pbds;
      using namespace std;


      /*** Typedef ***/
      typedef long long ll;
      typedef unsigned long long ull;

      template<class T>
      inline T fastIn()
      {
          register char c = 0;
          register T a = 0;
          bool neg = false;

          while(c < 33) c = getchar();

          if(c == '-') neg = true;
          else a = c - '0';

          while(c = getchar(), c > 33)
              a = a * 10 + (c - '0');

          return (neg? -a : a);
      }

      /*** Input ***/
      #define sci1(a) scanf("%d",&a)
      #define sci2(a,b) scanf("%d %d",&a,&b)
      #define scln1(a) scanf("%lld",&a)
      #define scln2(a,b) scanf("%lld %lld",&a,&b)
      #define scln3(a,b,c) scanf("%lld %lld %lld",&a,&b,&c)


      /*** Output ***/
      #define pf1(a) printf("%d\n",a)
      #define pf2(a,b) printf("%d %d\n",a,b)
      #define pfln1(a) printf("%lld\n",a)
      #define pfln2(a,b) printf("%lld %lld\n",a,b)


      /*** Loops ***/
      #define foR0(num) for(ll i = 0; i < num; i++)
      #define foR1(num) for(ll i = 1; i <= num; i++)
      #define foRev(num) for(ll i = num - 1; i >= 0; i--)
      #define rep(i, x, n) for (ll i = x, _n = (n); i < _n; ++i)
      #define forIn(arr, num) for(ll i = 0; i < num; i++) cin>>arr[i];
      #define forIn1(arr, num) for(ll i = 1; i <= num; i++) cin>>arr[i];
      #define vpnt(ans) for(ll i = 0; i < ans.size(); i++) cout << ans[i] << (i + 1 < ans.size() ? ' ' : '\n');
      #define apnt(arr, num) for(ll i = 0; i < num; i++) cout << arr[i] << (i + 1 < num ? ' ' : '\n');


      /*** Define Values ***/

      #define     ff                first
      #define     ss                second
      #define     re                return
      #define     MP                make_pair
      #define     pb                push_back
      #define     SZ(x)             ((ll) (x).size())


      #define     EPS               10E-10
      #define     mxx               100005
      #define     MOD               1000000007
      #define     iseq(a,b)         (fabs(a-b)<EPS)
      #define     PI                3.141592653589793238462643


      #define     Ceil(a,b)         (a+b-1)/b
      #define     gcd(a, b)         __gcd(a,b)
      #define     min3(a,b,c)       min(a,min(b,c))
      #define     max3(a,b,c)       max(a,max(b,c))
      #define     lcm(a, b)         ((a)/gcd(a,b))*(b)
      #define     min4(a,b,c,d)     min(d,min(a,min(b,c)))
      #define     max4(a,b,c,d)     max(d,max(a,max(b,c)))
      #define     input             freopen("input.txt","rt", stdin)
      #define     output            freopen("output.txt","wt", stdout)


      #define     all(v)            v.begin(),v.end()
      #define     mem(nam,val)      memset(nam, val, sizeof(nam))
      #define     ps(x,y)           fixed<<setprecision(y)<<x
      #define     for2D0(n,m)       for(ll i=0;i<n;i++)for(ll j=0;j<m;j++)
      #define     for2D1(n,m)       for(ll i=1;i<=n;i++)for(ll j=1;j<=m;j++)
      #define     Unique(X)         (X).resize(unique(all(X))-(X).begin())
      #define     get_pos(c,x)      (lower_bound(c.begin(),c.end(),x)-c.begin())
      #define     get_pos_up(c,x)   (upper_bound(c.begin(),c.end(),x)-c.begin())
      #define     IOS               ios_base::sync_with_stdio(false); cin.tie(NULL); cout.tie(NULL);
      #define     for2Dpnt(arr,n,m) for(ll i=0;i<n;i++){for(ll j=0;j<m;j++)cout<<arr[i][j]<<" ";cout<<endl;}


      /*** STLs ***/
      typedef vector <ll> vll;
      typedef set <ll> sll;
      typedef multiset <ll> msll;
      typedef queue <ll> qll;
      typedef stack <ll> stll;
      typedef map <ll, ll> mll;
      typedef pair <ll, ll> pll;
      typedef vector <pair <ll , ll> > vpll;


      /*** BitWise Operations
      ///int Set(int N,int pos){return N=N | (1<<pos);}
      ///int reset(int N,int pos){return N= N & ~(1<<pos);}
      ///bool check(int N,int pos){return (bool)(N & (1<<pos));}
      ***/


      /*** Grids
      ///const int fx[] = {+1,-1,+0,+0};
      ///const int fy[] = {+0,+0,+1,-1};
      ///const int fx[] = {+0,+0,+1,-1,-1,+1,-1,+1}; ///King's move
      ///const int fy[] = {-1,+1,+0,+0,+1,+1,-1,-1}; ///king's Move
      ///const int fx[] = {-2,-2,-1,-1,+1,+1,+2,+2}; ///knight's move
      ///const int fy[] = {-1,+1,-2,+2,-2,+2,-1,+1}; ///knight's move
      ***/


      /*** Functions
      ///transform(data.begin(), data.end(), data.begin(),[](unsigned char c){ return std::tolower(c); });
      ///typedef tree<int, null_type, less<int>, rb_tree_tag, tree_order_statistics_node_update> ordered_set;
      ///ll toint(string s){ll n=0,k=1;for(int i=s.size()-1; i>=0; i--){n += ((s[i]-'0')*k);k*=10;}return n;}
      ///string tostring(ll x){string s="";while(x){s += (x%10)+'0';x/=10;}reverse(s.begin(),s.end());return s;}
      ///bool sortinrev(const pair<ll,ll> &a,const pair<ll,ll> &b)return (a.first > b.first);
      ///prime[]={2,4,2,4,6,2} //start loop from 29 to do prime factorization
      ///auto it = lower_bound(my_multiset.begin(), my_multiset.end(), 3);
      ///const auto pos = distance(my_multiset.begin(), it);
      ///priority_queue< pll ,vector<pll>,greater<pll> >p;
      ///lower_bound(all(v),r+1)-lower_bound(all(v),l);
      ///cout<<*X.find_by_order(0)<<endl;
      ///cout<<X.order_of_key(-5)<<endl;
      ///set< pair<int,int> >s;
      ///pair<int,int> p={3,2};
      ///auto lb=lower_bound(s.begin(),s.end(),p);
      ///cout<<(*lb).first<<" "<<(*lb).second<<endl;
      ***/


      /*** Some Prints ***/
      #define en cout << '\n';
      #define no cout << "NO" << '\n'
      #define yes cout << "YES" << '\n'


      //__uint128_t
      ll A[mxx*10];
      ll B[mxx*10];


      int main()
      {
          IOS;
          ll tst=1;
          //cin>>tst;
          for(ll tt=1; tt<=tst; tt++)
          {
              //code





















          }


          return 0;
      }

  ```
  
  </blockquote>
  </details>
        
  <details><summary> Solution-2 </summary>
  <blockquote>

  ```c++
    int whatIsLove() {
      //Comment
    }
  ```
  
  </blockquote>
  </details>
  

</details>   

</details>


        
        
        
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
</details>      
      
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

  </details>
        
        
 
        
        
        
        
## Sieve of Eratosthenes <sup>[[1]](https://forthright48.com/sieve-of-eratosthenes-generating-primes/)</sup><sup>[[2]](https://cp-algorithms.com/algebra/sieve-of-eratosthenes.html)</sup>
<pre>
      - Sieve of Eratosthenes - forthright48[1]
      - Sieve of Eratosthenes - Cp Algorithm[2]
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

  </details>
        
        
        
        
        
        
        
        
        
        
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

  </details>        
        
        

        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
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

  </details>         
        
        
        
        
        
        
        
        
        
        
        
        
        
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

  </details>  
        
        
        
        
        
        
        
        
        
        
        
        
        
        
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

  </details>          
        
        
        
        
        
        
       
        
<h1 align="center">Combinactorics & Probability</h1>    
        
        
                
## Combinactorics <sup>[[1]](https://youtu.be/M8BYckxI8_U)</sup><sup>[[2]](https://betterexplained.com/articles/navigate-a-grid-using-combinations-and-permutations/)</sup><sup>[[3]](https://www.handakafunda.com/problems-on-grids-paths-and-chessboards-for-cat-exam/)</sup><sup>[[4]](https://youtu.be/mAvGUFlAJwQ)</sup><sup>[[5]](https://youtu.be/FuPM7OhGda0)</sup><sup>[[6]](https://www.topcoder.com/thrive/articles/Basics%20of%20Combinatorics)</sup><sup>[[7]](https://forthright48.com/prufer-code-linear-representation-of-a-labeled-tree/)</sup><sup>[[8]](https://forthright48.com/application-of-prufer-code-random-tree-generation-cayleys-formula-and-building-tree-from-degree-count/)</sup><sup>[[9]](https://medium.com/i-math/the-birthday-problem-307f31a9ac6f)</sup><sup>[[10]](https://medium.com/i-math)</sup><sup>[[11]](https://youtu.be/9vRUxbzJZ9Y)</sup>
<pre>
      - Art of Problem Solving: Counting Paths on a Grid - Youtube[1]
      - Navigate a Grid Using Combinations And Permutations - Better Explained[2]
      - Problems on Grids, Paths, and Chessboards for CAT Exam[3]
      - Combinatorics Introduction Correction: nCk = nC(n-k)[Bangla][4]
      - Probabilty + Combinatorics - Intermediate (BACS-BUBT National Programming Camp, 2017)[Bangla][5]
      - Basic of Combinatorics[6]
      - Prufer Code: Linear Representation of a Labeled Tree[7]
      - Application of Prufer Code: Random Tree Generation, Cayley’s Formula and Building Tree from Degree Count[8]
      - The Birthday Problem[9]
      - Medium Math[10]
      - The Monty Hall Problem[11]
</pre> 
### Problems
<details>
  <summary>Combinations - LightOj</summary>

  <blockquote>

  ```sh
  https://lightoj.com/problem/combinations
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```c++
      ll A[1000000];
      map<ll,vector<ll> >ps;
      void fact()
      {
          A[0]=A[1]=1;
          for(ll i=2;i<=1e6+2;i++)
          {
              A[i]=((A[i-1]%MOD)*i)%MOD;
          }
      }

      ll bigmod ( ll a, ll p, ll m )
      {
          ll res = 1;
          ll x = a;

          while ( p )
          {
              if ( p & 1 ) //p is odd
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
           fact();
           ll t;
           cin>>t;
           for(ll j=1;j<=t;j++)
           {
               ll n,r;
               cin>>n>>r;
               cout<<"Case "<<j<<": ";
               ll a=((A[n-r]%MOD)*(A[r]%MOD))%MOD;
               ll b=((A[n]%MOD)*(bigmod(a,MOD-2,MOD)))%MOD;
               cout<<b<<endl;
           }


          return 0;
      }
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>
      
<details>
  <summary>Good Predictions - SPOJ</summary>

  <blockquote>

  ```sh
 https://www.spoj.com/problems/GOODB/
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

  </details>
        
        
        
        
## Star Bars Theorem
## Bell Numbers
## The Coupon Collector's Problem
## Catalan Numbers
## Pascal's Triangle properties
## Stirling Number <sup>[[1]](https://youtu.be/yQCIAiA288s)</sup>
<pre>
      - What is Stirling Number of First Kind - Youtube[1]
</pre> 
### Problems
<details>
  <summary>No Name</summary>

  <blockquote>

  ```sh
  No link!!
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

  </details>
        
        
        
        
        
   
        
        
        
<h1 align="center">Theory & Function & Principle</h1> 
        
        
## Pigeonhole principle
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
<h1 align="center">Search</h1>     
        
## Binary Search <sup>[[1]](https://youtu.be/6ysjqCUv3K4)</sup><sup>[[2]](http://www.shafaetsplanet.com/?p=2279)</sup><sup>[[3]](https://www.programiz.com/dsa/binary-search)</sup>
<pre>
      - Introduction to Binary Search - Youtube[1]
      - বাইনারি সার্চ - Shafaet Blog[2]
      - Binary Search - Programiz[3]
</pre> 
### Problems
<details>
  <summary>The Playboy Chimp - UVA</summary>

  <blockquote>

  ```sh
  https://onlinejudge.org/index.php?option=onlinejudge&Itemid=8&page=show_problem&problem=1552
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

  </details>   
        
        
        
 
        
        
        
        
        
        
        
        
## Fraction Binary Search <sup>[[1]](https://github.com/ShahjalalShohag/code-library/blob/master/Miscellaneous/Fraction%20Binary%20Search.cpp)</sup>
<pre>
      - Introduction to Fraction Binary Search - Github[1]
</pre> 
### Problems
<details>
  <summary>Conductors - Timus</summary>

  <blockquote>

  ```sh
  https://acm.timus.ru/problem.aspx?space=1&num=1011
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

  </details> 
        
        
        
        
        
        
        
        
## Ternary Search <sup>[[1]](https://youtu.be/INa9L56heHE)</sup><sup>[[2]](https://eshafik.wordpress.com/2017/08/07/ternary-search/#more-161)</sup><sup>[[3]](https://cp-algorithms.com/num_methods/ternary_search.html)</sup>
<pre>
      - Searching an element in a sorted array (Ternary Search) - Youtube[1]
      - Introduction to Ternary Search - Shafik's Blog[2]
      - Ternary Search - Cp Algorithm[3]
</pre> 
### Problems
<details>
  <summary>Help Chokro - Toph</summary>

  <blockquote>

  ```sh
  https://toph.co/p/help-chokro
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

  </details>  
        
        
        
        
        
        
        
        
## Parallel Binary Search
        
        
        
        
        
        
        
        
        
        
        
        
        
<h1 align="center">Dynamic Programming</h1>     
        
        
## Basic DP
        
        
### Bangla
        
```sh
    https://sites.google.com/site/smilitude/recursion_and_dp    
```
        
```sh
   http://www.shafaetsplanet.com/planetcoding/?p=1022     
```
        
        
        
### Hindi
        
 ```sh
   https://youtube.com/playlist?list=PL_z_8CaSLPWekqhdCPmFohncHwz8TY2Go     
```
        
        
        
### English 
        
```sh
   https://www.codechef.com/certification/data-structures-and-algorithms/prepare#foundation   
```
        
```sh
   https://www.youtube.com/watch?v=OQ5jsbhAv_M&list=PLcDimPvbmfT8qAxD6JH_kmXiQwTNcoK78  
```
        
```sh
   https://codeforces.com/blog/entry/67679    
```
        
        
        
        
### Basic DP Problems
<details>
  <summary>Help Chokro - Toph</summary>

  <blockquote>

  ```sh
      https://toph.co/p/help-chokro
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
        
        
        
        
        
        
        
        
        
        
        
        
        
        
        
                
        
        

