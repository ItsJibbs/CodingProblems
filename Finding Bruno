# Author= Jibran Khan, Date= 5th June 2023, Problem= Finding Bruno

Direction=["north","east","south","west"]

Possible_position_list=[]

def Pos_right(direction,x,y,n):
    #right_turn
    
    global Possible_position
    #new_direction=Direction[Direction.index(direction)+1]
    if (n==0):
        pass
        
    elif (direction=="north"):
        try:
            Possible_position_list.remove([x,y])
        except ValueError:
            pass
        new_direction=Direction[1]
        x=x+1
        Possible_position_list.append([x,y])
        
        n=n-1
        
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    elif (direction=="east"):
        try:
            Possible_position_list.remove([x,y])
        except ValueError:
            pass
        new_direction=Direction[2]
        y=y-1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    elif (direction=="south"):
        try:
            Possible_position_list.remove([x,y])
        except ValueError:
            pass
        new_direction=Direction[3]
        x=x-1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    elif (direction=="west"):
        try:
            Possible_position_list.remove([x,y])
        except ValueError:
            pass
        new_direction=Direction[0]
        y=y+1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    

def Pos_left(direction,x,y,n):
    #left_turn
    global Possible_position
    #new_direction=Direction[Direction.index(direction)+1]
    if (n==0):
        pass
    elif (direction=="north"):
        new_direction=Direction[-1]
        x=x-1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    elif (direction=="east"):
        
        new_direction=Direction[0]
        y=y+1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    elif (direction=="south"):
        
        new_direction=Direction[1]
        x=x+1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    elif (direction=="west"):
        new_direction=Direction[2]
        y=y-1
        Possible_position_list.append([x,y])
        n=n-1
        Pos_right(new_direction,x,y,n)
        Pos_left(new_direction,x,y,n)
    
#input    
N=1

for i in Direction:
    Pos_right(i,0,0,N)
    Pos_left(i,0,0,N)

Possible_position_list1=[]    
Possible_position_list2=[Possible_position_list1.append(i) for i in Possible_position_list if i not in Possible_position_list1]    
print("Total possible positions are ",len(Possible_position_list1))   
print("Possible Cordinates of Bruno after {} minutes are :".format(N))
print(Possible_position_list1)
 
    
