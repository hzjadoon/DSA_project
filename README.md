Community Management System
This project implements a simple community management system using C++. It allows you to add, display, update, remove, sort, and search for members within a community.

Features
Add Member: Add a new member to the community.
Display Members: Display all members in the community.
Remove Member: Remove a member from the community by name.
Update Member Details: Update the age and role of an existing member.
Sort Members: Sort members by name, age, or role.
Search Members: Search for members by name, age, or role using a random selection method.
File Structure
main.cpp: Contains the main logic and menu-driven interface for interacting with the community.
members.txt: A file where member details are stored when added.
Classes
Member
Represents a community member.

Attributes:
string name
int age
string role
Methods:
Member(string name, int age, string role)
void updateDetails(int newAge, const string& newRole)
Node
Represents a node in the linked list.

Attributes:
Member member
Node* next
Methods:
Node(const Member& member)
Community
Manages the community as a linked list of members.

Attributes:
Node* head
Methods:
Community()
~Community()
void addMember(const string& name, int age, const string& role)
void displayMembers() const
void removeMember(const string& name)
void updateMember(const string& name, int newAge, const string& newRole)
void sortByName()
void sortByAge()
void sortByRole()
void randomSearch() const
void searchMemberByName(const string& name) const
void searchMemberByAge(int age) const
void searchMemberByRole(const string& role) const
Usage
Compile the Program:

sh
Copy code
g++ -o community main.cpp
Run the Program:

sh
Copy code
./community
Interact with the Menu:

Choose from the options to add, display, remove, update, sort, or search for members.
Follow the prompts to enter member details as needed.
Example
markdown
Copy code
1. Add Member
2. Display Members
3. Remove Member
4. Search Member (Random)
5. Update Member Details
6. Sort Members by Name
7. Sort Members by Age
8. Sort Members by Role
9. Exit
Enter your choice:

Notes
Ensure that members.txt is in the same directory as the executable to properly store and retrieve member details.
The program uses a linked list to manage the community members, ensuring efficient addition and removal of members.
License
This project is licensed under the MIT License. See the LICENSE file for details.
