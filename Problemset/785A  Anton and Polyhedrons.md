# 785A  Anton and Polyhedrons

https://codeforces.com/problemset/problem/785/A

# Solution

```
#include <bits/stdc++.h>
using namespace std;
 
int main()
{
    ios_base::sync_with_stdio(false);
    cin.tie(0);
    
    int n;
    cin >> n;
    int contador = 0;
    for(int i = 0; i < n; ++i){
        string s;
        cin >> s;
        if(s == "Tetrahedron") contador += 4;
        else if(s == "Cube") contador += 6;
        else if(s == "Octahedron") contador += 8;
        else if(s == "Dodecahedron") contador += 12;
        else if(s == "Icosahedron") contador += 20;
    }
 
    cout << contador << endl;
    return 0;
}
```