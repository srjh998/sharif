#include <iostream>
using namespace std;
template <typename S>
S calibratevalue(S &x,char factor){
    return x*factor;
}
int main() {
    int x=5;
    char factor=10;
    cout<<calibratevalue(x,factor)<<endl;
}
