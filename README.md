#include <iostream>
using namespace std;




int returnTotalBill()
{   char c;
    char items;
    int vegItems;
    int NonVeg;
    char SelectAgain;
    int billAmount=0;


    cout<<" --------------Welcome to Avengers restaurant---------------- "<<endl;
    cout<<"---------------Please follow the instructions---------------- \n"<<endl;
    cout<<" Step 1 : Please press s to start your order !\n"<<endl;
    cout<<" Step 2 : You can order both Veg and nonVeg as per your wish :)\n"<<endl;
    cout<<" step 3 : Please press a to order veg items from the menu :)\n "<<endl;
    cout<<" step 4 : Please press b to order nonVeg items from the menu :)\n "<<endl;
    cout<<"Note : you will get the your final bill after complete order !\n"<<endl;
    cout<<" Enter option : ";
    start:
    cin>>c;


    if(c=='s' || c=='S'){
        items:

       cout<<" Please enter your choice "<<endl;
       cout<<" (a): Veg items            (b):NonVeg items "<<endl<<" Enter option : ";

       cin>>items;
