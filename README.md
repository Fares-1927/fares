number_of_piles = int(input("enter tje total number of piles to play\n"))
k = 5
w = 0
x = 0
b = 0
z = number_of_piles

for j in range(0,number_of_piles):
    while k<8:
        x = float(input("enter your number player 1 \n"))
        y = int(x) ** 0.5
        if int(x) < x or int(y) < y or x > number_of_piles or int(x) > z or int(x) == 0:
            print("please enter non zero square integer number smaller than: " + str(z))
        else:
            break
    z = z - int(x)
    print("yhe reminder is " + str(z))

    if z == 0:
        print("player 1 is the winner")
        exit()
    else:
        pass

    while k<8:
        b = float(input("enter your number player 2: \n"))
        s = int(b) ** 0.5
        if int(b) < b or int(s) < s or b > number_of_piles or int(b) > z or b ==0:
            print("please enter non zero aquare integer number smaller than " + str(z))
        else:
            break
    w = z - int(b)
    print("the reminder is: " +str(w))
    if w == 0:
        print("player 2 is winner")
        exit()

        z = w
