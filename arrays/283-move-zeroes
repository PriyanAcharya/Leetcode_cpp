class Solution {
public:
    void moveZeroes(vector<int>& nums) {
        int lastNotZero = 0;

        for(int i =0 ; i< nums.size(); i++){
            if (nums[i] != 0){
                nums[lastNotZero++] = nums[i];
            }
        }

        for(int i = lastNotZero; i<nums.size(); i++){
            nums[i] = 0;
        }
    }
};
