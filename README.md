// Online C compiler to run C program online
#include <stdio.h>


   
char name[50];
char number[50];
int info = 0;

void createUser() {
    if (info == 0) {
        printf("\nEnter Name: ");
        scanf("%s", name);
        printf("Enter Phone Number: ");
        scanf("%s", number);
        info = 1;
        printf("User Created!\n");
    
    }
}

void readUser() {
    if (info == 1) {
        printf("\nName: %s\n", name);
        printf("Phone Number: %s\n", number);
    
    }
}

void updateUser() {
    if (info == 1) {
        printf("\nEnter New Name: ");
        scanf("%s", name);
        printf("Enter New Phone Number: ");
        scanf("%s", number);
        printf("User Updated!\n");
    
    }
}


int main() {
    int choice = 0;

    for(int d = 0; d>=choice; d++) {
        printf("\nCRUD Contact List\n");
        printf("1. Create\n");
        printf("2. Read\n");
        printf("3. Update\n");
        printf("Enter your choice: ");
        scanf("%d", &choice);
        

        switch (choice) {
            case 1:
                createUser();
                break;
            case 2:
                readUser();
                break;
            case 3:
                updateUser();
                break;
            default:
                printf("\nInvalid!");
        }
    }

  











    return 0;
}
