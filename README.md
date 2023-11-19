# Sum-of-Unique-Element-using-Java-Leetcode

    class Solution {
        public int sumOfUnique(int[] nums) {
           int sum =0;
           for(int num: nums){
               if(isUnique(nums,num)) sum+=num;
           }
           return sum;
        }
        public boolean isUnique(int[] nums,int num){
            int count=0;
            for(int value:nums){
                if(value==num){
                    count++;
                };
            }
            return count==1;
        }
    }
