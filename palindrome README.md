# Test_Code
class Solution {
public: 
    bool isPalindrome(int x) {
        if(x < 0)
            return false;
        long int num = x, rv = 0, rm = 0;
        while(x != 0)
        {
            rm = x%10;
            rv = rv*10 + rm;
            x =x/10;
        }
        if(num == rv)
            return true;   
        else
            return false;
    
    }
};
