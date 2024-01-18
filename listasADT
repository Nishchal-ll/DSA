#include<iostream>
using namespace std;
#define max 10

class array{
public:
    int arr[max];
    int count;
    int n;
    int pos;
    int temp;

    void makeempty(){
        count=-1;
    }

    int isempty(){
        if(count<0){
            return 1;
        }
        else{
            return 0;
        }
    }

    int isfull(){
        if((count+1)==10){
            return 1;
        }else{
        return 0;
        }
    }

    void insertdata(){
        if(isempty()){
            cout<<"Data can't be entered"<<endl;
        }
        else{
           cout<<"Enter the number of data you want to add"<<endl;
           cin>>n;
           for(int i=0;i<n;i++){
            cout<<"Enter data number: "<<i<<endl;
            count++;
            cin>>arr[i];
           }
        }
    }


    void deletedata(){
        cout<<"Enter the position you want to delete"<<endl;
        cin>>pos;
        temp=arr[pos];
        arr[pos]=arr[n-1];
        arr[n-1]=temp;
        cout<<"Datas are: "<<endl;
        for(int i=0;i<n-1;i++){
                cout<< arr[i]<<endl;
    }

    }


    void traverse(){
        cout<<"Datas are"<<endl;
          for(int i=0;i<n;i++){
                cout<< arr[i]<<endl;
    }
    }
};
int main(){
    array a1;
    int g;
    do{
	cout<<"Menu"<<endl;
	cout<<"Press 1 to make the data empty"<<endl;
	cout<<"Press 2 to check the data is empty or not"<<endl;
	cout<<"Press 3 to check the data is full or not"<<endl;
	cout<<"Press 4 to insert the data"<<endl;
	cout<<"Press 5 to delete the data"<<endl;
	cout<<"Press 6 to see the list "<<endl;
	cout<<"Press any other key to exit"<<endl;
			cin>>g;
		switch(g){
			case 1:
			    a1.makeempty();
			    break;

            case 2:
            if(a1.isempty()){
			cout<<"Data is empty"<<endl;
	}
	else{
		cout<<"Data is not empty"<<endl;
	}
	break;

	          case 3:
				if(a1.isfull()){
			cout<<"Data is full"<<endl;
	}
	else{
		cout<<"Data is not full"<<endl;
	}
	break;

	case 4:
		a1.insertdata();
		break;

		case 5:
			a1.deletedata();
			break;

			case 6:
				a1.traverse();
				break;

				default:
					g=7;


}
}while(g!=7);
return 0;
}

