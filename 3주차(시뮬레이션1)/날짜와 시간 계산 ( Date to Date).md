```c++
#include <iostream>
using namespace std;
int main() {
    // 여기에 코드를 작성해주세요.
    int m1,m2,d1,d2;
    cin >> m1 >> d1 >> m2 >> d2;
    int num_of_days[13] = {0, 31, 28, 31, 30, 31, 30, 31, 31, 30, 31, 30, 31};
    int days = 1;
    while (true){
        if(m1 == m2 && d1 == d2){ // 날짜와 시간이 같아지면 탈출
            break;
        }
        d1++;
        days++;

        if(d1 > num_of_days[m1]){
            m1++;
            d1 = 1;
        }

    }
    cout << days;
    return 0;
}
```
