class Solution {
    public int lengthOfLastWord(String s) {
        int a=s.length()-1;
    	int sum=0;
    	for(int i=a;i>=0;i--)
    	{
    		if(s.charAt(i)!=' '){
    			sum++;
                }
    		else if(s.charAt(i)==' ')
    		{
    			if(sum!=0)
                break;
    		}
    	}
    	return sum;	

    }
}
