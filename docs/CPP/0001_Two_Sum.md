
``` C++
class Solution
{
public:
	std::vector<int> twoSum(std::vector<int>&nums, int target)
	{
		std::vector<int> Ans;
		for (int i = 0; i < nums.size() - 1; i++)
		{
			for (int j = i + 1; j < nums.size(); j++)
			{
				if (nums[i] + nums[j] == target)
				{
					Ans.push_back(i);
					Ans.push_back(j);
					return Ans;
				}
			}
		}
		return Ans;
	}
};
```