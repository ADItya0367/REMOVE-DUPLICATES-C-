# REMOVE-DUPLICATES-C-

**Intuition****
Brute Force Technique

**Approach**
-* cheak weather the array is empty or not if empty return -1
-* declare i=0; and j
-* run another looop for j where j=0;j<nums.size();j++
-* if nums[i]!=nums[j]
-* i++ increase the count
-* else nums[i]==nums[j]
-* return i+1;

**Complexity**
**Time complexity:**
o(n)
**Space complexity:**
o(n)
**Code**
class Solution {
public:
    int removeDuplicates(vector<int>& nums) {
    if(nums.size()==0)
    return 0;
    int i=0;
    int j; 
    for(j=1;j<nums.size();j++)
    {  
      if(nums[i]!=nums[j])
        {
            i++;

        } 
        nums[i]=nums[j];
    }  
    return i+1;
    }
};
