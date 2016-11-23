# test

import java.util.*;

/**
 * Created by yuji5 on 2016/11/22.
 */
public class Main {
    private  static int M ;
    private static int N ;//矩阵大小小
    public static void main(String args[]){
       
        Scanner in = new Scanner(System.in);
        M = in.nextInt();
        N = in.nextInt();
        int[][] ori_matrix = new int[M][N];
 //       int[][] out_matrix = new int[N][M];
        in.nextLine();
        for(int m = 0;m < M ;m++){
            for(int n = 0;n < N ;n++){
                ori_matrix[m][n] = in.nextInt();
            }
            in.nextLine();
        }
        for(int n = 0;n < N ;n++){
            for(int m = M-1;m >= 0;m--){
                System.out.print(ori_matrix[m][n]+" ");
            }
            System.out.println();
        }
    }
}
