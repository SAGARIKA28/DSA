// Determine if a string has all Unique Characters

// It can be done easily by using a map to check this, but it will take O(N) space
//Here we will do it using no extra space using bit manipulatio. P.S: This is only applicaple if we only consider a-z only.
//TC: o(N), SC: O(1)

public class Main
{
	public static void main(String[] args) {
		String word = "abcdefah";
		if(isUnique(word)){
		    System.out.print("Is Unique");
		}
		else{
		    System.out.print("Is not unique");
		}
		
	}
  // fucntion to check if a word has unique char or not
	public static boolean isUnique(String w){
	    int checker = 0; // this is of size 32 bit, it will act like a map, each index will tell if that char is present or not in it's respective position.
		for(int i=0;i<w.length();i++)
		{
		    int val = w.charAt(i) - 'a'; // finding out the index of that value. suppose if 'a' is the char, it's positon will be 0
		    if((checker & (1<<val)) > 0){ // when you and checker and 1<<val(putting 1 in char's respecting place) >0 which means, the char is already there
		       return false;
		    }
		     checker = checker | 1<<val; // if not present, put the value there
		}
		return true;
	}
}
