# DSA-Practice-Questions

Problem statement
You are given a number ’n’.



Find the number of digits of ‘n’ that evenly divide ‘n’.



Note:
A digit evenly divides ‘n’ if it leaves no remainder when dividing ‘n’.


Example:
Input: ‘n’ = 336

Output: 3

Explanation:
336 is divisible by both ‘3’ and ‘6’. Since ‘3’ occurs twice it is counted two times.


using namespace std;
int countDigits(int n){
	cin>>n;
  int count=0;
    int z= n;
    while(n>0){
    
        int x=n%10;
         if(x==0){
          count += 0;
        }
       else if (z % x == 0) {
          count += 1; 
        }
        
   n = n / 10;
	
    }
	return count;
}

