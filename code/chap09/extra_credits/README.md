# Submit your extra credit in this folder
#include <iostream>
#include <iomanip>
using namespace std;

void print_tree(int n){
    if (n<1) {return ;}
    print_tree(n-1);
    cout<<setw(n*' ')<<"This was written by call number "<<n<<endl;    
}

void print_tree2(int n){
    if (n<1) {return ;}
    cout<<setw(n*' ')<<"This ALSO written by call number "<<n<<endl;
    print_tree2(n-1);
}

int main()
{
    print_tree(4);
    print_tree2(4);
    return 0;
}
