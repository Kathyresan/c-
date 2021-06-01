#include <iostream>
using namespace std;

char space(40);
int main()
{   cout<<"________________________________________________"<<endl<<endl;
    cout<<"|           # Grade Determiner #               |"<<endl;
    cout<<"|            Company ANONYMOUS                 |"<<endl;
    cout<<"|                                              |"<<endl;
    cout<<"________________________________________________"<<endl<<endl<<endl;

float mark,A,B,C,D,E,F;

cout<<"Please enter the mark: ";
cin>>mark;
cout<<"\n";


if (mark>79)
{
    cout<<"Excellent!"<<endl;
    cout<<"Your grade is A  ^_^"<<endl;
}

else if (mark>64)
{
    cout<<"Good!"<<endl;
    cout<<"Your grade is B  *_*"<<endl;
}

else if (mark>49)
{
    cout<<"Satisfactory!"<<endl;
    cout<<"Your grade is C  +_+"<<endl;
}

else if (mark>39)
{
    cout<<"Pass!"<<endl;
    cout<<"Your grade is D  -_-"<<endl;
}

else if (mark>=0)
{
    cout<<"Fail!"<<endl;
    cout<<"Your grade is E  "<<endl;
}

cout<<"\n";
cout<<"Thank You"<<endl;

 return 0;

}
