#include<iostream>
using namespace std;
struct node
{
    int data;
    struct node *next;
};
class stack
{
    struct node *top;
    public:
    stack()
    {
        top=NULL;
    }
    void push(); 
    void pop();  
    void show(); 
};
void stack::push()
{
    int value;
    node *ptr;
    cout<<"\nPUSH Operationn";
    cout<<"Enter a number to insert: ";
    cin>>value;
    ptr=new node;
    ptr->data=value;
    ptr->next=NULL;
    if(top!=NULL)
        ptr->next=top;
    top=ptr;
    cout<<"\nNew node is inserted to the stack!";

}
void stack::pop()
{
    struct node *temp;
    if(top==NULL)
    {
        cout<<"\nEmpty Stack";
    }
    temp=top;
    top=top->next;
    delete temp;
}
void stack::show()
{
    struct node *ptr1=top;
    cout<<"\nThe stack is\n";
    while(ptr1!=NULL)
    {
        cout<<ptr1->data<<" ->";
        ptr1=ptr1->next;
    }
    cout<<"NULL\n";
}

int main()
{
    stack s;
    int choice=1;
    while(choice!=4)
    {
        cout<<"\n\t\tSTACK USING LINKED LIST\n\n";
        cout<<"1:PUSH\n2:POP\n3:DISPLAY STACK\n4:EXIT";
        cout<<"\nEnter your choice(1-4): ";
        cin>>choice;
        switch(choice)
        {
            case 1:
                s.push();
                break;
            case 2:
                s.pop();
                break;
            case 3:
                s.show();
                break;
            case 4:
                break;
            default:
                cout<<"Incorrect choice!";
                break;
        }
    }
    return 0;
}
