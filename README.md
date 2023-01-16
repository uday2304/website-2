def tic_tac_toe(): 
    board = [[1,2,3],[4,5,6],[7,8,9]] 
    print("\nWelcome to tic tac toe! You will be playing against the computer.\n") 
    turn = True 
    while(True): 
        if turn: # user's turn 
            print("Your turn") 
            move = int(input("Enter your move (1-9):")) 
            board[move//3][move%3-1] = 'X' 
            for row in board:
                print(row) 

            turn=False 
