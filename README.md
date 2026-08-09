# Number-System-Converter.
DESCRIPTION:- 
The Number System Converter is a Python application that converts numbers between different number systems, including Binary, Decimal, Octal, and Hexadecimal. The user selects the input number system, enters a value, and the program displays its equivalent in all other number systems.
CODE:-
while True:
    print("\n===== Number System Converter =====")
    print("1. Decimal")
    print("2. Binary")
    print("3. Octal")
    print("4. Hexadecimal")
    print("5. Exit")

    choice = input("Enter your choice: ")

    if choice == "1":
        num = int(input("Enter Decimal number: "))
        print("Binary      :", bin(num)[2:])
        print("Octal       :", oct(num)[2:])
        print("Hexadecimal :", hex(num)[2:].upper())

    elif choice == "2":
        num = input("Enter Binary number: ")
        decimal = int(num, 2)
        print("Decimal     :", decimal)
        print("Octal       :", oct(decimal)[2:])
        print("Hexadecimal :", hex(decimal)[2:].upper())

    elif choice == "3":
        num = input("Enter Octal number: ")
        decimal = int(num, 8)
        print("Decimal     :", decimal)
        print("Binary      :", bin(decimal)[2:])
        print("Hexadecimal :", hex(decimal)[2:].upper())

    elif choice == "4":
        num = input("Enter Hexadecimal number: ")
        decimal = int(num, 16)
        print("Decimal     :", decimal)
        print("Binary      :", bin(decimal)[2:])
        print("Octal       :", oct(decimal)[2:])

    elif choice == "5":
        print("Thank you!")
        break

    else:
        print("Invalid choice. Please try again.")
  SAMPLE INPUT:-
  ===== Number System Converter =====
1. Decimal
2. Binary
3. Octal
4. Hexadecimal
5. Exit

Enter your choice: 1
Enter Decimal number: 25

SAMPLE OUTPUT:-
Binary      : 11001
Octal       : 31
Hexadecimal : 19

FEATURES:-
*Converts Decimal to Binary, Octal, and Hexadecimal.
*Converts Binary to Decimal, Octal, and Hexadecimal.
*Converts Octal to Decimal, Binary, and Hexadecimal.
*Converts Hexadecimal to Decimal, Binary, and Octal.
*Simple menu-driven interface.
*Handles multiple conversions until the user exits.
