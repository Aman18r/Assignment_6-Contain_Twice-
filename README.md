# Assignment_6-Contain_Twice-

import java.util.Scanner;

public class Main{
    public static boolean containsTwice(int[] nums, int a){
        for(int i=0; i<a; i++){
            for(int j=0; j<a; j++){
                if(nums[i] == nums[j] ){
                    return true;
                }
            }
        }
        return false;
    }

    public static void main(String[] args) {
        Scanner sc = new Scanner(System.in);
        System.out.println("Enter the size of an array:");
        int a = sc.nextInt();
        int[] arr = new int[a];
        for(int i=0; i<a; i++){
            arr[i] = sc.nextInt();
        }
        if(containsTwice(arr,a)){
            System.out.println("True");
        }
        else{
            System.out.println("False");
        }
    }
}
