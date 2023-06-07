-#by Ganer@scameror$
-  import random
a=[1,2,3]
a1=[4,5,6]
a2=[7,8,9]
s=[1,4,7]
s1=[2,5,8]
s2=[3,6,8]
k=[a,a1,a2]
l=[s,s1,s2]
A_v=[1,2,3,4,5,6,7,8,9]
recoder=0
user_numbers=[]
def u(w,h,o=a,l=a1,p=a2):
    if  w in o:
        if h in o:
            return True
    elif w in l:
        if h in l:
            return True
    elif w in p:
        if h in p:
            return True
while len(A_v) != 0:


    current_number = int(input("123 "))
    A_v.remove(current_number)
    user_numbers.append(current_number)
    recoder += 1
    if recoder==1 and current_number!=9:
        print(current_number+1)
        A_v.remove(current_number+1)
        continue
    elif recoder==1:
        print(current_number-1)
        A_v.remove(current_number-1)
        continue

    if current_number+2 in user_numbers:
        pass
        if current_number + 1 in A_v and   u(current_number+1,current_number+2):
            print(current_number + 1)
            A_v.remove(current_number + 1)
            continue


        else:
            pass
    if current_number+1 in user_numbers:
        pass
        if current_number + 2 in A_v and u(current_number+1,current_number+2):
            print(current_number + 2)
            A_v.remove(current_number + 2)
            continue
        if current_number -1 in user_numbers:
            pass
            if current_number - 2 in A_v and   u(current_number-1,current_number-2):
                print(current_number - 2)
                A_v.remove(current_number - 2)
                continue
        if current_number -2 in user_numbers:
            pass
            if current_number -1 in A_v and   u(current_number-2,current_number-1):
                print(current_number -1)
                A_v.remove(current_number -1)
                continue


        else:
            pass
    if current_number+3 in user_numbers:
        pass
        if current_number + 6 in A_v and   u(current_number+3,current_number+6):
            print(current_number + 6)
            A_v.remove(current_number + 6)
            continue


        else:
            pass
    if current_number+6 in user_numbers:
        pass
        if current_number + 3 in A_v and  u(current_number+6,current_number+3):
            print(current_number + 3)
            A_v.remove(current_number + 3)
            continue


        else:
            pass
    if current_number-3 in user_numbers:
        pass
        if current_number - 6 in A_v and  u(current_number-3,current_number-6)  :
            print(current_number - 6)
            A_v.remove(current_number - 6)
            continue
        elif  current_number + 6 in A_v and  u(current_number+6,current_number-3)  :
            print(current_number + 6)
            A_v.remove(current_number + 6)
            continue


        else:
            pass
    if current_number + 1 in user_numbers:
        pass
        if current_number - 1 in A_v and   u(current_number+1,current_number-1) :

            print(current_number - 1)
            A_v.remove( current_number- 1)
            continue

        else:
            pass
    if current_number - 1 in user_numbers:
        pass
        if current_number + 1 in A_v and   u(current_number-1,current_number+1):
            print(current_number + 1)
            A_v.remove(+ 1)
            continue
    if current_number + 3 in user_numbers:
            pass
            if current_number - 3 in A_v and   u(current_number+3,current_number-3):
                print(current_number - 3)
                A_v.remove(- 3)
                continue

    else:
       pass
    if current_number - 3 in user_numbers:
        pass
        if current_number + 3 in A_v and  u(current_number-3,current_number+3):
            print(current_number + 3)
            A_v.remove(+ 3)
            continue

    else:
        pass


    if current_number - 6 in user_numbers:
        pass
        if current_number - 3 in A_v and   u(current_number-6,current_number-3):
            print(current_number - 3)
            A_v.remove(current_number - 3)
            continue


        elif  current_number - 3 in A_v and  u(current_number-3,current_number-6):
            print(current_number + 3)
            A_v.remove(current_number + 3)
            continue

            pass
    if current_number == 1:
        if current_number + 4 in user_numbers:
            if current_number + 8 in A_v:
                print(current_number + 8)
                A_v.remove(current_number + 8)
                continue
            else:
                pass
        if current_number + 8 in user_numbers:
            if current_number + 4 in A_v:
                print(current_number + 4)
                A_v.remove(current_number + 4)
                continue
            else:
                pass
    else:
        pass
    if current_number == 7:
        if current_number -2 in user_numbers:
            if current_number -4 in A_v:
                print(current_number -4)
                A_v.remove(current_number -4)
                continue
            else:
                pass
        if current_number - 8 in user_numbers:
            if current_number - 4 in A_v:
                print(current_number - 4)
                A_v.remove(current_number - 4)
                continue
            else:
                pass
    else:
        pass


    if current_number == 9:
        if current_number - 4 in user_numbers:
            if current_number - 8 in A_v:
                print(current_number - 8)
                A_v.remove(current_number - 8)
                continue
            else:
                pass
        if current_number - 8 in user_numbers:
            if current_number - 4 in A_v:
                print(current_number - 4)
                A_v.remove(current_number - 4)
                continue
            else:
                pass
    else:
        pass
    if current_number==5:

        if current_number +4 in user_numbers:
         if current_number - 4 in A_v:
            print(current_number - 4)
            A_v.remove(current_number - 4)
            continue
         else:
            pass
        if current_number - 4 in user_numbers:
            if current_number + 4 in A_v:
                print(current_number + 4)
                A_v.remove(current_number + 4)
                continue
            else:
                pass
    if current_number == 3:
        if current_number + 4 in user_numbers:
            if current_number + 4 in A_v:
                print(current_number + 4)
                A_v.remove(current_number + 4)
                continue
            else:
                pass
        if current_number + 4 in user_numbers:
            if current_number + 2 in A_v:
                print(current_number + 2)
                A_v.remove(current_number + 2)
                continue
            else:
                pass
    if current_number==5 and 4 in user_numbers:
        if  9 in A_v:
            print(9)
            A_v.remove(9)
    a =True
    while True:
        l=random.randint(1,10)
        if l in A_v:
            print(l)
            A_v.remove(l)
            break

        else:
            continue

