#include <iostream>
#include <string>

using namespace std;
float Malaysia,India,Japan,China,US,Thailand,Nepal,Korea,malaysia_time,choice,hour,minute,number;
char name[30];
char space(40);
int main()
{

char response;
do{

char name[30];


cout<<"\n";
cout<<" |                                           |"<<endl;
cout<<" |Welcome to the Malaysia time zone converter|"<<endl;
cout<<" |             # BLACK HAT #                 |"<<endl;
cout<<" |                 ^_^                       |"<<endl<<endl<<endl;


cin.ignore();
string names;
cout<<" Enter your name : ";
getline(cin,names);
cout<<"\n";
cout<< " Hello " <<names<<endl<<endl;




cout<<" 1) Enter time (24 hours)"<<endl<<endl;
cout<<" 2) Exit"<<endl<<endl;



cout<<" Please choose option 1 or 2: ";
cin>>choice;
cout<<"\n";


if (choice==1)
{


   cout<<" You have chosen option 1 "<<endl<<endl;
   cout<< " Enter the time (hours): ";
   cin>>hour;
   cout<< " Enter the time (minute): ";
   cin>>minute;
   cout<<"\n";

   cout<< " Your current time is: "<<hour<< ":" <<minute<<endl<<endl<<endl<<endl;

}



if (choice==2)
{
   cout<<" You have chosen option 2 "<<endl<<endl;
   cout<<" Thank you , Have a nice day"<<endl<<endl<<endl;
   return 0;
}




cout<<" Here are lists of countries that you can change time"<<endl<<endl;

cout<< "1) India"<<endl;
cout<< "2) Japan"<<endl;
cout<< "3) China"<<endl;
cout<< "4) US"<<endl;
cout<< "5) Thailand"<<endl;
cout<< "6) Nepal"<<endl;
cout<< "7) Korea"<<endl;

cout<< "\nPlease enter the number: ";
cin>>number;
cout<<"\n";


if (number == 1)
{
    hour=hour-2;
    minute=minute-30;

    if (hour >= 24)
{
    hour=hour-24;
}

if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;
    minute=minute+60;
}

    cout<< "Your time in India will be: "<<hour<< ":" <<minute<<endl;
}

else if (number == 2)
{
     hour=hour+1;
     minute=minute;

     if (hour >= 24)
{
    hour=hour-24;
}

if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;
    minute=minute+60;
}

     cout<< "Your time in Japan will be: "<<hour<< ":" <<minute<<endl;
}
else if (number == 3)
{
    hour=hour;
    minute=minute;

    if (hour >= 24)
{
    hour=hour-24;
}if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;
    minute=minute+60;
}

    cout<< "Your time in China will be: "<<hour<< ":" <<minute<<endl;
}

else if (number == 4)
{
    hour=hour-12;
    minute=minute;

    if (hour >= 24)
{
    hour=hour-24;
}

if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;
    minute=minute+60;
}

    cout<< "Your time in US will be: "<<hour<< ":" <<minute<<endl;
}

else if (number == 5)
{
    hour=hour-1;
    minute=minute;
    if (hour >= 24)
{
    hour=hour-24;
}

if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;
    minute=minute+60;
}

    cout<< "Your time in Thailand will be: "<<hour<< ":" <<minute<<endl;
}

else if (number == 6)
{
    hour=hour-2;
    minute=-15;
    if (hour >= 24)
{
    hour=hour-24;
}

if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;
    minute=minute+60;
}

    cout<< "Your time in Nepal will be: "<<hour<< ":" <<minute<<endl;
}

else if (number == 7)
{
    hour=hour+1;
    minute=minute;
    if (hour >= 24)
{
    hour=hour-24;
}

if (hour < 0)
{
    hour=hour+24;
}
if (minute>=60)
{
    minute=minute-60;
    hour=hour+1;

}

if (minute<0)
{
    hour=hour-1;

    minute=minute+60;
}

    cout<< "Your time in Korea will be: "<<hour<< ":" <<minute<<endl;
}
 cout<<"\n";
 cout<<"Do you want to continue (y/n): ";
 cin>>response;


}while (response=='y' || response=='Y' );


cout<<"\nThank you , Have a nice day!"<<endl;


return 0;
}

