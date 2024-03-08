# Stutern


 import json

def load_contacts():
    try:
        with open("contacts.json", "r") as f:
            contacts = json.load(f)
    except FileNotFoundError:
        contacts = {}
    return contacts

def save_contacts(contacts):
    with open("contacts.json", "w") as f:
        json.dump(contacts, f, indent=4)

def add_contact(name, phone):
    contacts = load_contacts()
    contacts[name] = phone
    save_contacts(contacts)
    print("Contact added successfully!")

def view_contacts():
    contacts = load_contacts()
    if contacts:
        print("Contacts:")
        for name, phone in contacts.items():
            print(f"{name}: {phone}")
    else:
        print("No contacts found.")

def main():
    print("Welcome to your Digital Diary!")
    while True:
        print("\n1. Add a new contact\n2. View contacts\n3. Exit")
        choice = input("What would you like to do? (Enter a number): ")
        if choice == "1":
            name = input("Enter the name of the contact: ")
            phone = input("Enter the phone number of the contact: ")
            add_contact(name, phone)
        elif choice == "2":
            view_contacts()
        elif choice == "3":
            print("Goodbye!")






            import json

def load_contacts():
    try:
        with open("contacts.json", "r") as f:
            contacts = json.load(f)
    except FileNotFoundError:
        contacts = {}
    return contacts

def save_contacts(contacts):
    with open("contacts.json", "w") as f:
        json.dump(contacts, f, indent=4)

def add_contact(name, phone):
    contacts = load_contacts()
    contacts[name] = phone
    save_contacts(contacts)
    print(f"Contact '{name}' with phone number '{phone}' has been added successfully!")

def view_contacts():
    contacts = load_contacts()
    if contacts:
        print("\nYour Contacts:")
        for name, phone in contacts.items():
            print(f"Name: {name}, Phone: {phone}")
    else:
        print("You haven't added any contacts yet.")

def main():
    print("Welcome to Your Digital Diary!")
    while True:
        print("\nWhat would you like to do?")
        print("1. Add a new contact")
        print("2. View contacts")
        print("3. Exit")
        choice = input("Please enter the number of your choice: ")
        if choice == "1":
            name = input("Enter the name of the contact: ")
            phone = input("Enter the phone number of the contact: ")
            add_contact(name, phone)
        elif choice == "2":
            view_contacts()
        elif choice == "3":
            print("Thank you for using Your Digital Diary. Goodbye!")
            break
        else:
            print("Sorry, I didn't understand that. Please enter a valid number.")

if __name__ == "__main__":
    main()




Digital Diary Script

import json

def load_contacts():
    try:
        with open("contacts.json", "r") as f:
            contacts = json.load(f)
    except FileNotFoundError:
        contacts = {}
    return contacts

def save_contacts(contacts):
    with open("contacts.json", "w") as f:
        json.dump(contacts, f, indent=4)

def add_contact(name, phone):
    contacts = load_contacts()
    contacts[name] = phone
    save_contacts(contacts)
    print(f"A new contact '{name}' with phone number '{phone}' has been added to your diary!")

def view_contacts():
    contacts = load_contacts()
    if contacts:
        print("\nYour Contacts:")
        for name, phone in contacts.items():
            print(f"Name: {name}, Phone: {phone}")
    else:
        print("Your diary is empty. Add some contacts to see them here!")

def main():
    print("Welcome to Your Digital Stutern!")
    while True:
        print("\nWhat would you like to do?")
        print("1. Add a new contact")
        print("2. View contacts")
        print("3. Exit")
        choice = input("Please enter the number of your choice: ")
        if choice == "1":
            name = input("Enter the name of the new contact: ")
            phone = input("Enter the phone number of the new contact: ")
            add_contact(name, phone)
        elif choice == "2":
            view_contacts()
        elif choice == "3":
            print("Thank you for using Your Digital Diary. Goodbye!")
            break
        else:
            print("I didn't understand that. Please enter a valid number.")

if __name__ == "__main__":
    main()


README for Digital Diary
Dear Stutern,

Welcome to Your Digital Diary! This little script helps you keep track of your contacts in a simple and organized way.

How to Use:

Adding a New Contact:

Choose option 1.
Enter the name and phone number of the new contact when prompted.
Viewing Contacts:

Choose option 2 to see all your saved contacts.
Exiting:

Simply choose option 3 to exit the diary.
That's it! Your contacts will be saved automatically for your next visit.

Enjoy keeping your contacts organized with Your Digital Diary!

With love,
Olumide Buari
            break
        else:
            print("Invalid input. Please enter a valid number.")

if __name__ == "__main__":
    main()




Version Control with Git
Dear Stutern,

I've decided to use Git to keep track of the changes in our Digital Diary script. This will help us manage different versions and collaborate more effectively.

Steps:

Initialize Git Repository:

Open the terminal and navigate to the directory containing our Digital Diary script.
Run the command git init to initialize a new Git repository.
Add Changes:

Whenever we make changes to the script, we'll add them to the staging area using git add <filename>.
Commit Changes:

After adding the changes, we'll commit them with a meaningful message using git commit -m "Message":
Example: git commit -m "Add functionality to view contacts"
View Commit History:

We can view the commit history using git log to see all the changes and their corresponding messages.
Collaboration:

If we're working with others, we'll push our changes to a remote repository using git push and pull changes from the remote repository using git pull.
README Updates:

We'll keep our README file updated with clear instructions on how to use the Digital Diary script and any changes made in each version.
That's it! With Git, we can easily manage our code changes and keep our project organized.

With love,
Olumide Buari

README for Digital Diary
Dear Diary,

Welcome to Your Digital Diary! This little script helps you keep track of your contacts in a simple and organized way.

How to Use:

Adding a New Contact:

Choose option 1.
Enter the name and phone number of the new contact when prompted.
Viewing Contacts:

Choose option 2 to see all your saved contacts.
Exiting:

Simply choose option 3 to exit the diary.
Version History:

Version 1.0:

Initial release with basic functionality.
Added options to add and view contacts.
Version 1.1:

Improved user interface for better readability.
Bug fixes and performance improvements.
That's it! Your contacts will be saved automatically for your next visit.

Enjoy keeping your contacts organized with Your Digital Diary!

With love,
Olumide Buari





