# Binary_To_Decimal
In this repository i have written code for converting Binary number to Decimal number






#include<bits/stdc++.h>
using namespace std;
class Solution
{
	public:
		int binary_to_decimal(string str)
		{
		   string num = str;
    int Dec = 0,b=1,len = num.length();
    for (int i = len - 1; i >= 0; i--) {
        if (num[i] == '1')
            Dec += b;
        b*=2;
    }

    return Dec;
		}
};

int main(){
    int T;
    cin >> T;
    while(T--)
    {
    	string str;
    	cin >> str;
    	Solution ob;
    	int  ans = ob.binary_to_decimal(str);
    	cout << ans <<"\n";
    }
	return 0;
} 
