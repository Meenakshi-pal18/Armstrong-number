# Armstrong-number
// User function Template for C++
class Solution {
  public:
    bool armstrongNumber(int n) {
        // code here
        int sum=0;
        int dup=n;
        while(n>0){
            int x=n%10;
            sum=sum+(x*x*x);
            n=n/10;
        }
        if(dup==sum){
            return true;
            //cout<<"true";
        }
        else{
            return false;
            //cout<<"false";
        }
    }
};
