# Data-structure-practic# Stack Overflow and Underflow Check

stack = []
max_size = 3

def push():
    if len(stack) >= max_size:
        print("Stack Overflow")
    else:
        item = int(input("Enter element to push: "))
        stack.append(item)
        print(item, "pushed into stack")

def pop():
    if len(stack) == 0:
        print("Stack Underflow")
    else:
        item = stack.pop()
        print(item, "popped from stack")

while True:
    print("\n1.Push  2.Pop  3.Display  4.Exit")
    choice = int(input("Enter choice: "))

    if choice == 1:
        push()
    elif choice == 2:
        pop()
    elif choice == 3:
        print("Stack:", stack)
    elif choice == 4:
        break
    else:
        print("Invalid choice")al-program-23
