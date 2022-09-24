# Loop-to-Increment-a-Variable
# We will use FOR Loop to Increment a Variable through a Range.
# Input Format: You will be given two positive integers, a and b (a<=b), separated by a newline.
# Output Format: For each integer  in the inclusive interval [a,b] :
# If 1<=n<=9 , then print the English representation of it in lowercase. That is "one" for 1, "two" for 2, and so on.
# Else if n>9 and it is an even number, then print "even".
# Else if n>9 and it is an odd number, then print "odd".


#include <iostream>
#include <cstdio>
using namespace std;

int main() {
    // Complete the code.
    int a,b,i;
    cin>>a>>b;
    string num[11] ={"one","two","three","four","five","six","seven","eight","nine"};
    for(i=a;i<=b;i++){
        if (i>9 && i%2!=0){
            cout<<"odd"<<endl;
        }
        else if(i>9 && i%2==0){
            cout<<"even"<<endl;;
        }
        else{
            cout<<num[i-1]<<endl;
        }
    }
    
    return 0;
}
