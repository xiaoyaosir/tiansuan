#include <iostream>
#include <algorithm>
using namespace std;
int a[9] = {1,2,3,4,5,6,7,8,9};
bool judge()
{
    if(a[0]*100+a[1]*10+a[2]+a[3]*100+a[4]*10+a[5] == a[6]*100+a[7]*10+a[8])
        return true;
    return false;
}
int main()
{
    int count = 0;
    do
    {
        if(judge())
            count++;
    }while(next_permutation(a,a+9));
    cout << count << endl;
    return 0;
}
