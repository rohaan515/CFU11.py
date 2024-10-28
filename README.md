def print_multiples_of_ten():
    for i in range(10, 81, 10):
        print(i)

def print_floats():
    for i in range(0, 21):
        print(i / 2)

def sing_bottles_of_beer():
    for i in range(99, 0, -1):
        print(f"{i} bottle{'s' if i > 1 else ''} of beer on the wall, {i} bottle{'s' if i > 1 else ''} of beer.")
        print("Take one down, pass it around, " + (f"{i-1} bottle{'s' if i-1 > 1 else ''} of beer on the wall.\n" if i > 1 else "no more bottles of beer on the wall.\n"))

def main():
    while True:
        print("Choose an option:")
        print("1: Print multiples of ten up to 70")
        print("2: Print numbers from 0 to 10 in increments of 0.5")
        print("3: Sing the 99 Bottles of Beer song")
        print("4: Exit")
        choice = input("Enter your choice: ")

        if choice == '1':
            print_multiples_of_ten()
        elif choice == '2':
            print_floats()
        elif choice == '3':
            sing_bottles_of_beer()
        elif choice == '4':
            break
        else:
            print("Invalid choice, please try again.")

if __name__ == "__main__":
    main()# CFU11.py
