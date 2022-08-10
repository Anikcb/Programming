<h1 align="center">Graph</h1>

## Breadth-first Search <sup>[[1]](https://www.youtube.com/watch?v=pcKY4hjDrxk)</sup><sup>[[2]](http://www.shafaetsplanet.com/?p=604)</sup><sup>[[3]](https://cp-algorithms.com/graph/breadth-first-search.html)</sup>
<pre>
      - Graph Traversals - Youtube[1]
      - Breadth-first Search - Cp Algorithm[2]
      - Breadth-first Search - Shafaet Planet[3]
</pre>
### Problems

<details>
  <summary> NAKANJ - SPOJ </summary>

  <blockquote>
  

  ```sh
  https://www.spoj.com/problems/NAKANJ/
  ```
     
        
<details>

  <summary>Solutions</summary>
  

  <details><summary> Solution-1 </summary>
  <blockquote>

  ```c++
      #include<bits/stdc++.h>
      #include<time.h>
      #include <iomanip>
      using namespace std;

      #define          ll                     long long int
      #define          EPS                    10E-10
      #define          ull                    unsigned long long int
      #define          db                     double
      #define          pii                    pair < int, int>
      #define          pll                    pair < ll, ll>
      #define          MOD                    1000000007
      #define          mxx                    100005
      #define          vi                     vector<int>
      #define          vl                     vector<ll>
      #define          pb                     push_back
      #define          sc                     scanf
      #define          pf                     printf
      #define          ff                     first
      #define          ss                     second
      #define          re                     return
      #define          QI                     queue<int>
      #define          SI                     stack<int>
      #define          iseq(a,b)              (fabs(a-b)<eps)
      #define          SZ(x)                  ((int) (x).size())
      #define          scin(x)                scanf("%d",&(x))
      #define          scin2(x,y)             scanf("%d %d",&(x),&(y))
      #define          scln(x)                scanf("%lld",&(x))
      #define          scln2(x,y)             scanf("%lld %lld",&(x),&(y))
      #define          scch1(ch)              scanf("%s",ch)
      #define          scch2(ch1,ch2)         scanf("%s %s",ch1,ch2)
      #define          min3(a,b,c)            min(a,min(b,c))
      #define          min4(a,b,c,d)          min(d,min(a,min(b,c)))
      #define          max3(a,b,c)            max(a,max(b,c))
      #define          max4(a,b,c,d)          max(d,max(a,max(b,c)))
      #define          ms(a,b)                memset(a,b,sizeof(a))
      #define          gcd(a, b)              __gcd(a,b)
      #define          lcm(a, b)              ((a)*(b)/gcd(a,b))
      #define          input                  freopen("input.txt","rt", stdin)
      #define          output                 freopen("output.txt","wt", stdout)
      #define          PI                     3.141592653589793238462643
      #define          rep( i , a , b )       for( i=a ; i<b ; i++)
      #define          rev( i , a , b )       for( i=a ; i>=b ; i--)
      #define          repx( i ,a,b, x)       for( i=a ; i<b ; i+=x)
      #define          RUN_CASE(t,T)          for(__typeof(t) t=1;t<=T;t++)
      #define          zero(a)                memset(a,0,sizeof a)
      #define          all(v)                 v.begin(),v.end()
      #define          get_pos(c,x)           (lower_bound(c.begin(),c.end(),x)-c.begin())
      #define          CASEL(t)               printf("Case %d:\n",t)
      #define          Unique(X)             (X).erase(unique(all(X)),(X).end())

      void FLASH() {ios_base::sync_with_stdio(false); cin.tie(NULL); cout.tie(NULL);}
      void SETF() {cout.ios_base::setf(ios_base::fixed); cerr.ios_base::setf(ios_base::fixed);}
      void UNSETF() {cout.ios_base::unsetf(ios_base::fixed); cerr.ios_base::unsetf(ios_base::fixed);}

      bool sortinrev(const pair<ll,ll> &a,const pair<ll,ll> &b)
      {
          return (a.first > b.first);
      }

      ///--------------Graph Moves--------------------------------------
      ///const int fx[] = {+1,-1,+0,+0};
      ///const int fy[] = {+0,+0,+1,-1};
      ///const int fx[] = {+0,+0,+1,-1,-1,+1,-1,+1}; ///King's move
      ///const int fy[] = {-1,+1,+0,+0,+1,+1,-1,-1}; ///king's Move
      const int fx[] = {-2,-2,-1,-1,+1,+1,+2,+2}; ///knight's move
      const int fy[] = {-1,+1,-2,+2,-2,+2,-1,+1}; ///knight's move
      ///---------------------------------------------------------------

      ///-----------------------Bitmask------------------
      ///int Set(int N,int pos){return N=N | (1<<pos);}
      ///int reset(int N,int pos){return N= N & ~(1<<pos);}
      ///bool check(int N,int pos){return (bool)(N & (1<<pos));}
      ///------------------------------------------------

      ll A[1000000];
      ll B[1000000];
      map<ll, vector<ll> > node;

      ll row=8,col=8;
      ll d[10][10],vis[10][10];
      void bfs(ll sx,ll sy,ll dx,ll dy)
      {
          memset(vis,0,sizeof vis);
          vis[sx][sy]=1;
          queue<pii>q;
          q.push(pii(sx,sy));
          while(!q.empty())
          {
              pii top=q.front();
              q.pop();
              for(ll k=0; k<8; k++)
              {
                  ll tx=top.ff+fx[k],ty=top.ss+fy[k];
                  if(tx>=0 && tx<row && ty>=0 && ty<col  && vis[tx][ty]==0)
                  {
                      vis[tx][ty]=1;
                      d[tx][ty]=d[top.ff][top.ss]+1;
                      q.push(pii(tx,ty));
                  }
              }
          }
          cout<<d[dx][dy]<<endl;


      }


      int main()
      {
           FLASH();
      #ifndef ONLINE_JUDGE
           time_t time_t1, time_t2;
           time_t1 = clock();
      #endif
           //Start
           ll t;
           cin>>t;
           while(t--)
           {
               ll y1,y2;
               char x1,x2;
               cin>>x1>>y1>>x2>>y2;
               bfs(x1-'a',y1-1,x2-'a',y2-1);
               zero(vis);zero(d);
           }








      #ifndef ONLINE_JUDGE
        time_t2 = clock();
        SETF();
        cerr<<"Time taken: "<<setprecision(7)<<(time_t2 - time_t1)/(double)CLOCKS_PER_SEC<<"\n";
        UNSETF();
      #endif



          return 0;
      }

  ```
  
  </blockquote>
  </details>
  </details>
</details>
       
        
        
<details>
  <summary> AKBAR - SPOJ </summary>

  <blockquote>

  ```sh
   https://www.spoj.com/problems/AKBAR/
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
   https://github.com/Anikcb/Spoj_practice
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>
      
      
      
      
      

    
    
       
<details>
  <summary> MICEMAZE - SPOJ </summary>

  <blockquote>

  ```sh
   https://www.spoj.com/problems/MICEMAZE/
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
   https://github.com/Anikcb/Spoj_practice
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>  
    
    
    
    
    
    
    
    
    
<details>
  <summary> SPIKES - SPOJ </summary>

  <blockquote>

  ```sh
   https://www.spoj.com/problems/SPIKES/
  ```
        
 <details>

  <summary>Solution</summary>
  
  <blockquote>
  
  ```sh
   https://github.com/Anikcb/Spoj_practice
  ```
  </blockquote>
  </details>      
      
      
      
 </blockquote>
</details>

  </details>
    
    
    
    
    
    
<details>
  <summary> Shortest Path - CODEFORCES </summary>

  <blockquote>

  ```sh
   https://codeforces.com/contest/59/problem/E
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
    
    
    
    
    
    
    
    


# MultiSource BFS
- [Christmas Trees](https://codeforces.com/contest/1283/problem/D)
- [Nearest Opposite Parity](https://codeforces.com/contest/1272/problem/E)
- [BITMAP](https://www.spoj.com/problems/BITMAP/)
- [SNSOCIAL](https://www.codechef.com/SNCKPB17/problems/SNSOCIAL/)
