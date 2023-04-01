class Solution {
public:
    int maximumCostSubstring(string s, string chars, vector<int>& vals) {
        
        int arr[26] = {0};
        
        for(int i=0; i<s.size(); i++) {
            arr[s[i] - 97] = s[i] - 96;
        }
        
        for(int i=0; i<chars.size(); i++) {
            arr[chars[i] - 97] = vals[i];
        }
        
        int ans = 0;
        int sum = 0;
        
        for(int i=0; i<s.size(); i++) {
            sum += arr[s[i] - 97];
            if(sum <= 0) {
                sum = 0;
            }
            else if(sum > ans) ans = sum;
        }
        
        return ans;
        
    }
};
