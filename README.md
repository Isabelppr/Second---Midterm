# Second---Midterm
def start_game():                                                                                                                     
    print("You wake up in a dark cave, unsure of how you got there. Two paths lie ahead:")
    print("1. Go left: A narrow, dark tunnel with the sound of rushing water.")
    print("2. Go right: A wider passage with mysterious light and whispers.")
    choice1 = input("Choose your path (left/right): ").lower()

    if choice1 == "left":
        narrow_tunnel()
    elif choice1 == "right":
        wide_passage()
    else:
        print("Invalid choice. Please choose 1. left or 2.right")
        start_game()

def narrow_tunnel():
    print("\nYou enter the dark tunnel and soon find a raging underground river.")
    print("1. Swim across the river.")
    print("2. Search for a bridge.")
    choice2 = input("Do you swim or search for a bridge? (swim/bridge): ").lower()

    if choice2 == "swim":
        print("\nAs you swim, a giant squid emerges from the water! You cast 'Stupefy' and escape!")
        triwizard_task()
    elif choice2 == "bridge":
        print("\nYou find a bridge, but a dragon guards it! You cast 'Expelliarmus' to disarm the dragon’s fire breath and make it across!")
        triwizard_task()
    else:
        print("Invalid choice. Please choose 1. left or 2.right")
        narrow_tunnel()

def wide_passage():
    print("\nYou enter the wider passage. A glowing magical altar stands before you, offering great power.")
    print("1. Accept the dark magic.")
    print("2. Refuse the offer and move on.")
    choice3 = input("Do you accept or refuse the magic? (accept/refuse): ").lower()

    if choice3 == "accept":
        print("\nYou feel immense power surging through you, but soon Voldemort appears!")
        print("Captured by Voldemort, you are enslaved by dark magic. FAIL.")
    elif choice3 == "refuse":
        print("\nYou refuse the dark magic. The cave begins to collapse, and you run!")
        triwizard_task()
    else:
        print("Invalid choice. Please choose 1. left or 2.right")
        wide_passage()

def triwizard_task():
    print("\nYou find yourself in the final task of the Triwizard Tournament: a magical maze!")
    print("1. Go left: Toward eerie fog.")
    print("2. Go right: Toward an opening with distant sounds of battle.")
    choice4 = input("Which way do you go? (left/right): ").lower()

    if choice4 == "left":
        print("\nThe fog hides a blast-ended skrewt! You barely escape its fiery attack.")
        print("You emerge victorious from the maze and win the Triwizard Tournament! VICTORY.")
    elif choice4 == "right":
        print("\nYou find yourself in the midst of Death Eaters! Voldemort casts the 'Avada Kedavra' curse!")
        print("You couldn’t escape. FAIL.")
    else:
        print("Invalid choice. Try again.")
        triwizard_task()