```c++
#include <iostream>
using namespace std;
int main() {
    // 여기에 코드를 작성해주세요.
    int a,b,c,d;
    int hour,mins;
    cin >> a >> b >> c >> d;

    hour = (c - a)*60;

    if(b > d){
        mins = (60 - b) + d;
        hour = hour - 60;

    }
    else{
        mins = d - b;
    }
    
    cout << hour + mins ;
    return 0;
}
```
