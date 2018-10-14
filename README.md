public int maxTriple(int[] nums) {
  
  int firstValue = nums[0];
  int middleValue = nums[nums.length/2];
  int lastValue = nums[nums.length-1];
  
  if(nums.length == 1){
    return nums[0];
  }

  else{
    if(firstValue > middleValue && firstValue > lastValue){
      return firstValue;
    }
    else if(middleValue > firstValue && middleValue > lastValue){
      return middleValue;
    }
    else{
      return lastValue;
    }
  }

}
