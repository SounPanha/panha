#include<iostream>
#include<conio.h>
using namespace std;
class student{
	private :
		int id;
		string name;
		string sex;
		string major;
		float s1,s2,s3,s4,s5;
		public :
			void Personal()
			{
				cout<<"========================Personal======================"<<endl;
				cout<<"Enter Student ID =";cin>>id;
				cout<<"Enter Student Name =";cin>>name;
				cout<<"Enter Student Gender =";cin>>sex;
				cout<<"Enter Student Major =";cin>>major;
			}
			void Subject()
			{
				cout<<"========================Subject==================="<<endl;
				cout<<"C++ =";cin>>s1;
				cout<<"Data Structur =";cin>>s2;
				cout<<"DataBase =";cin>>s3;
				cout<<"English =";cin>>s4;
				cout<<"Data communication =";cin>>s5;
			}
			int Sum()
			{
				return s1+s2+s3+s4+s5;
			}
			void Head_per()
			{
				cout<<"========================Result======================"<<endl;
				cout<<">>>>>>>>>>>>>>>>>>>>>>>>Personal<<<<<<<<<<<<<<<<<<<<"<<endl;
				cout<<"ID\tName\tGender\tMajor\t"<<endl;
			}
			void Head_sub()
			{
				cout<<">>>>>>>>>>>>>>>>>>>>>>>>Subject<<<<<<<<<<<<<<<<<<<<<"<<endl;
				cout<<"C++\tData Structur\tDataBase\tEnglish\tData Communication\t\tTotal"<<endl;
			}
			void Out_per()
			{
				cout<<id<<"\t"<<name<<"\t"<<sex<<"\t"<<major<<"\t"<<endl;
			}
			void Out_sub()
			{
				cout<<s1<<"\t"<<s2<<"\t"<<s3<<"\t\t\t"<<s4<<"\t\t\t"<<s5<<"\t\t"<<Sum()<<"\t"<<endl;
			}
};
int main()
{
	student class1;
	class1.Personal();
	class1.Subject();
	class1.Head_per();
	class1.Out_per();
	class1.Head_sub();
	class1.Out_sub();
	getch();
	
}
