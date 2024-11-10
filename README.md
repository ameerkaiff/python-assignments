#three python asssignments....

# Citizenship Verification and Document Check

is_citizen = input("Are you a citizen of India? (yes/no): ").lower() == "yes"

if is_citizen:
    print("You are confirmed as a citizen.")
    
    has_adhar = input("Do you have an Aadhaar card? (yes/no): ").lower() == "yes"
    birth_certificate = input("Do you have a birth certificate? (yes/no): ").lower() == "yes"
    voter_id = input("Do you have a Voter ID card? (yes/no): ").lower() == "yes"
    has_parents_passport = input("Do your parents have a passport? (yes/no): ").lower() == "yes"
    
    if has_adhar or birth_certificate or voter_id or has_parents_passport:
        print("You have the required documents to apply for a passport.")
        print("You can proceed with the process.")
    else:
        print("You don't have the required documents.")
        print("You can't proceed with the process.")
else:
    print("You are not a citizen of India.")

# Age Category Checker

while True:
    age = int(input("Enter your age: "))
    
    if age <= 13:
        print("You are a child.")
    elif 13 < age <= 18:
        print("You are a teenager.")
    elif 18 < age <= 30:
        print("You are a young adult.")
    elif 30 < age <= 50:
        print("You are an adult.")
    elif 50 < age <= 100:
        print("You are a senior citizen.")
    else:
        print("Please enter a valid age.")



# Department Identifier by Name

while True:
    name = input("Enter your name or enter 'o' to exit: ").lower()
    
    if name == "o":
        print("The program ends here.")
        break
    elif name == "ameer":
        print("You are from CSE.")
    elif name == "yousuf":
        print("You are from ECE.")
    elif name == "salman":
        print("You are from Civil Engineering.")
    elif name == "mateen":
        print("You are from CSE B section.")
    elif name == "nusary":
        print("You are from CSE A section.")
    elif name == "nadeem":
        print("You are from Civil Engineering.")
    elif name == "saif":
        print("You are from AIML.")
    else:
        print("Invalid name.")
