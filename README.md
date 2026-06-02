# Demo-4class Solution {
 public:
  int climbStairs(int n) {
    // dp[i] := the number of ways to climb to the i-th stair
    vector<int> dp(n + 1);
    dp[0] = 1;
    dp[1] = 1;
    for (int i = 2; i <= n; ++i)
      dp[i] = dp[i - 1] + dp[i - 2];
    return dp[n];
  }
};
88. Merge Sorted Array
class Solution {
 public:
  void merge(vector<int>& nums1, int m, vector<int>& nums2, int n) {
    int i = m - 1;      // nums1's index (the actual nums)
    int j = n - 1;      // nums2's index
    int k = m + n - 1;  // nums1's index 
      else
        nums1[k--] = nums2[j--]  }
};





okkk class Solution {
public:
    int minimumCost(vector<int>& cost) {
        // Sort the array in descending order to prioritize buying expensive items first
        sort(cost.rbegin(), cost.rend());
      
        int totalCost = 0;
      
        // Process items in groups of 3
        // Buy 2 items and get the 3rd one free (skip every 3rd item)
        for (int i = 0; i < cost.size(); i += 3) {
            // Add the first item in the group
class Solution {
public:
    vector<int> plusOne(vector<int>& digits) {
        for (int i = digits.size() - 1; i >= 0; --i) {
            ++digits[i];
            digits[i] %= 10;
            if (digits[i] != 0) return digits;
        }
        digits.insert(digits.begin(), 1);
        return digits;
    }
};
