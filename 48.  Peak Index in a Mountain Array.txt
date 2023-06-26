class Solution {
    public int peakIndexInMountainArray(int[] arr) {
        int ans = 0;
        int res = 0;
        for(int i = 0 ; i<arr.length; i++){
            if(arr[i]>ans){
                ans = arr[i];
            }
        }
        for(int i = 0 ;i < arr.length ; i++){
            if(arr[i]==ans){
                res = i;
            }
        }
        return res;

    }
}