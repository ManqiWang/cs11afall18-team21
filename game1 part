import java.util.Scanner;

public class projectVersion1 {
  public static void main(String[] args){
    System.out.println("Welcome to my Gomoku game");
    System.out.println("The game is designed for two player, each input their decision by turns");
    System.out.println("Please tpye your move in form of \"row,column\"");
    System.out.println("For example, if I want to place at the center, I just type in 7,7");
    Scanner sc = new Scanner(System.in);
    char a = '\u5341';
    char b = '\u2605';
    char c = '\u2606';
    boolean IsThereAWinner = false;
    int [][] BoardinInt = {
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
      {0,0,0,0,0,0,0,0,0,0,0,0,0},
    };
    //printboard
    {
      System.out.println("  1 2 3 4 5 6 7 8 9 10111213");
      for (int i = 0;i<BoardinInt.length;i++){
        int abc =i+1;
        if (abc<10){
          System.out.print(abc+ " ");
        }else{
          System.out.print(abc);
        }
        for (int j = 0; j<BoardinInt[i].length;j++){
          if (BoardinInt[i][j]==0){
            System.out.print(a);
          }else if (BoardinInt[i][j]==1){
            System.out.print(b+" ");
          }else if (BoardinInt[i][j]==2){
            System.out.print(c+" ");
          }
        }
        System.out.println();
      }
    }

    //Player1Move
    System.out.println("Player 1 move");
    String Move1 = sc.nextLine();
    String [] arr1 = Move1.split(",");
    int [] array1 = new int [2];
    array1[0] = Integer.parseInt(arr1[0]);
    array1[1] = Integer.parseInt(arr1[1]);
    BoardinInt [array1[0]-1][array1[1]-1]= 1;

    //printboard
    System.out.println("  1 2 3 4 5 6 7 8 9 10111213");
    for (int i = 0;i<BoardinInt.length;i++){
      int abc =i+1;
      if (abc<10){
        System.out.print(abc+ " ");
      }else{
        System.out.print(abc);
      }
      for (int j = 0; j<BoardinInt[i].length;j++){
        if (BoardinInt[i][j]==0){
          System.out.print(a);
        }else if (BoardinInt[i][j]==1){
          System.out.print(b+" ");
        }else if (BoardinInt[i][j]==2){
          System.out.print(c+" ");
        }
      }
      System.out.println();
    }

    //player2move
    System.out.println("Player 2 move");
    String Move2 = sc.nextLine();
    String [] arr2 = Move2.split(",");
    int [] array2 = new int [2];
    array2[0] = Integer.parseInt(arr2[0]);
    array2[1] = Integer.parseInt(arr2[1]);
    BoardinInt [array2[0]-1][array2[1]-1]= 2;

    //printboard
    System.out.println("  1 2 3 4 5 6 7 8 9 10111213");
    for (int i = 0;i<BoardinInt.length;i++){
      int abc =i+1;
      if (abc<10){
        System.out.print(abc+ " ");
      }else{
        System.out.print(abc);
      }
      for (int j = 0; j<BoardinInt[i].length;j++){
        if (BoardinInt[i][j]==0){
          System.out.print(a);
        }else if (BoardinInt[i][j]==1){
          System.out.print(b+" ");
        }else if (BoardinInt[i][j]==2){
          System.out.print(c+" ");
        }
      }
      System.out.println();
    }
    int counter =1;
    while(!IsThereAWinner){

      if (counter%2 == 1){
        //Player1Move
        System.out.println("Player 1 move");
        Move1 = sc.nextLine();
        arr1 = Move1.split(",");
        array1 = new int [2];
        array1[0] = Integer.parseInt(arr1[0]);
        array1[1] = Integer.parseInt(arr1[1]);
        BoardinInt [array1[0]-1][array1[1]-1]= 1;

        //printboard
        System.out.println("  1 2 3 4 5 6 7 8 9 10111213");
        for (int i = 0;i<BoardinInt.length;i++){
          int abc =i+1;
          if (abc<10){
            System.out.print(abc+ " ");
          }else{
            System.out.print(abc);
          }
          for (int j = 0; j<BoardinInt[i].length;j++){
            if (BoardinInt[i][j]==0){
              System.out.print(a);
            }else if (BoardinInt[i][j]==1){
              System.out.print(b+" ");
            }else if (BoardinInt[i][j]==2){
              System.out.print(c+" ");
            }
          }
          System.out.println();
        }
        counter = counter+1;

        //is there a winner
        //vertical
        for (int horiz1 = 0;horiz1<13;horiz1++){
          for (int ver1 = 0;ver1<9;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1][ver1+1]&&BoardinInt[horiz1][ver1+2]==BoardinInt[horiz1][ver1+1]&&BoardinInt[horiz1][ver1+2]==BoardinInt[horiz1][ver1+3]&&BoardinInt[horiz1][ver1+3]==BoardinInt[horiz1][ver1+4]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
        //horizontal
        for (int horiz1 = 0;horiz1<9;horiz1++){
          for (int ver1 = 0;ver1<13;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1+1][ver1]&&BoardinInt[horiz1+2][ver1]==BoardinInt[horiz1+1][ver1]&&BoardinInt[horiz1+2][ver1]==BoardinInt[horiz1+3][ver1]&&BoardinInt[horiz1+3][ver1]==BoardinInt[horiz1+4][ver1]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
        // \
        for (int horiz1 = 0;horiz1<9;horiz1++){
          for (int ver1 = 0;ver1<9;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1+1][ver1+1]&&BoardinInt[horiz1+2][ver1+2]==BoardinInt[horiz1+1][ver1+1]&&BoardinInt[horiz1+2][ver1+2]==BoardinInt[horiz1+3][ver1+3]&&BoardinInt[horiz1+3][ver1+3]==BoardinInt[horiz1+4][ver1+4]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
        // /
        for (int horiz1 = 4;horiz1<13;horiz1++){
          for (int ver1 = 0;ver1<9;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1-1][ver1+1]&&BoardinInt[horiz1-2][ver1+2]==BoardinInt[horiz1-1][ver1+1]&&BoardinInt[horiz1-2][ver1+2]==BoardinInt[horiz1-3][ver1+3]&&BoardinInt[horiz1-3][ver1+3]==BoardinInt[horiz1-4][ver1+4]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
      }else{
        //player2move
        System.out.println("Player 2 move");
        Move2 = sc.nextLine();
        arr2 = Move2.split(",");
        array2 = new int [2];
        array2[0] = Integer.parseInt(arr2[0]);
        array2[1] = Integer.parseInt(arr2[1]);
        BoardinInt [array2[0]-1][array2[1]-1]= 2;
        counter= counter + 1;
        //printboard
        System.out.println("  1 2 3 4 5 6 7 8 9 10111213");
        for (int i = 0;i<BoardinInt.length;i++){
          int abc =i+1;
          if (abc<10){
            System.out.print(abc+ " ");
          }else{
            System.out.print(abc);
          }
          for (int j = 0; j<BoardinInt[i].length;j++){
            if (BoardinInt[i][j]==0){
              System.out.print(a);
            }else if (BoardinInt[i][j]==1){
              System.out.print(b+" ");
            }else if (BoardinInt[i][j]==2){
              System.out.print(c+" ");
            }
          }
          System.out.println();


        //is there a winner
        //vertical
        for (int horiz1 = 0;horiz1<13;horiz1++){
          for (int ver1 = 0;ver1<9;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1][ver1+1]&&BoardinInt[horiz1][ver1+2]==BoardinInt[horiz1][ver1+1]&&BoardinInt[horiz1][ver1+2]==BoardinInt[horiz1][ver1+3]&&BoardinInt[horiz1][ver1+3]==BoardinInt[horiz1][ver1+4]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
        //horizontal
        for (int horiz1 = 0;horiz1<9;horiz1++){
          for (int ver1 = 0;ver1<13;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1+1][ver1]&&BoardinInt[horiz1+2][ver1]==BoardinInt[horiz1+1][ver1]&&BoardinInt[horiz1+2][ver1]==BoardinInt[horiz1+3][ver1]&&BoardinInt[horiz1+3][ver1]==BoardinInt[horiz1+4][ver1]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
        // \
        for (int horiz1 = 0;horiz1<9;horiz1++){
          for (int ver1 = 0;ver1<9;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1+1][ver1+1]&&BoardinInt[horiz1+2][ver1+2]==BoardinInt[horiz1+1][ver1+1]&&BoardinInt[horiz1+2][ver1+2]==BoardinInt[horiz1+3][ver1+3]&&BoardinInt[horiz1+3][ver1+3]==BoardinInt[horiz1+4][ver1+4]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
        // /
        for (int horiz1 = 4;horiz1<13;horiz1++){
          for (int ver1 = 0;ver1<9;ver1++){
            if (BoardinInt[horiz1][ver1]==BoardinInt[horiz1-1][ver1+1]&&BoardinInt[horiz1-2][ver1+2]==BoardinInt[horiz1-1][ver1+1]&&BoardinInt[horiz1-2][ver1+2]==BoardinInt[horiz1-3][ver1+3]&&BoardinInt[horiz1-3][ver1+3]==BoardinInt[horiz1-4][ver1+4]&&BoardinInt[horiz1][ver1]!=0){
              IsThereAWinner = true;
            }
          }
        }
      }
      }
    }
    System.out.println("You Win");
  }
}
