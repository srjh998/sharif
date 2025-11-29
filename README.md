#include <iostream>
using namespace std;
template <typename S>
S calibratevalue(S &x, char factor){
    return x*factor;
    
}
void adjustReading(double *value, double offset){
    *value=*value+offset;
}

int main() {
    int x=5;
    char factor=10;
    double value;
    double offset=1.25;
    cout<<calibratevalue(x,factor)<<endl;
    cout<<"input a value"<<endl;
    cin>>value;
    adjustReading(&value,offset);
    cout<<value<<endl;
}
