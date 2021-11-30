#include <iostream>
#include <stdlib.h>     
#include <time.h>       
using namespace std;




int main(){
	 
	int numbers[1000];
	
	srand (time(NULL));
	for(int i=0;i<1000;i++){
		 numbers[i] = rand() % 100 + 1;
	}

	int countSix=0;
	for(int i=0;i<1000;i++){
		if(numbers[i]==6){
			countSix++;	
		}
	}
	cout<<countSix<<" times the number 6 appears in the array." << endl<< endl;
	system("pause");
	return 0;
}
