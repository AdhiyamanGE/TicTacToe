"""
00 01 02 
1  2  3 
10 11 12
4  5  6 
20 21 22
7  8  9

"""
def print_board(board):
    for i in range(0,3):
        for j in range(0,3):
            print(board[i][j]," ",end="")
        print()
    

def freele(board):
    for i in range(0,3):
        for j in range(0,3):
            if(board[i][j]=="*"):
                board[i][j]=b 
                return
            else:
                flag=0
    if(flag==0):
        return 0

def opi(board):
    

a="X"
b="O"
ls=[["*","*","*"],["*","*","*"],["*","*","*"]]
cd={
    "1":"00","2":"01","3":"02","4":"10","5":"11","6":"12","7":"20","8":"21","9":"22"
}

flag=1
while(flag!=0):
    inp=input("enter")
    x=(int)(cd[inp])
    ls[(int)(x/10)][(int)(x%10)]="X"
    freele(ls)
    
    print_board(ls)
