
class Solution {
public:
    vector<int> findMissingAndRepeatedValues(vector<vector<int>>& grid) {
        int n = grid.size();
        int total = n * n;

        unordered_set<int> seen;
        int sum_actual = 0;
        int duplicate = -1;

        for (auto& row : grid) {
            for (int val : row) {
                if (seen.count(val)) {
                    duplicate = val;
                } else {
                    seen.insert(val);
                }
                sum_actual += val;
            }
        }

        int expected_sum = total * (total + 1) / 2;
        int missing = expected_sum - (sum_actual - duplicate);

        return {duplicate, missing};
    }
};
