# Welcome to MkDocs

For full documentation visit [mkdocs.org](https://www.mkdocs.org).

## Commands

* `mkdocs new [dir-name]` - Create a new project.
* `mkdocs serve` - Start the live-reloading docs server.
* `mkdocs build` - Build the documentation site.
* `mkdocs -h` - Print help message and exit.

## Project layout

    mkdocs.yml    # The configuration file.
    docs/
        index.md  # The documentation homepage.
        ...       # Other markdown pages, images and other files.


# 问题概述

# 解题思路

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