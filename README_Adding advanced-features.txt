
CODE COMPLIATION:

In linux or ubuntu Environment 
use command g++ ML_assignment1.cpp 

In windows Environment open program in IDE and compile it.

CODE EXECUTION:

In ubuntu or linux Environment run the following commands to execute :
Command line inputs:
1. Training data file Path(like : c:\users\sandeep\train1.dat)
2. Testing Data file Path (Like : c:\users\sandeep\test1.dat)

./a.out train_data_file_path test_data_path 
 
To redirect output to a file, use the following command.
./a.out train_data_path test_data_path  > output_filename.txt

In windows Environment after compling the program an new excutable will be generated.

Run the Executable using the following command:
ML_assignment1.exe train_data_path test_data_path.

To redirect output to a file, use the following command.
ML_assignment1.exe train_data_path test_data_path > output_filename.txt

OUTPUT:
 After the above command is executed from the command prompt user is asked to enter a value that is either 1 or 2.
 
 If user enters 1 then the tree is constructed using ID3 algorithm.
 If user enters 2 then the tree is constructed using random attribute selection algorithm.
 
Program displays tree constructed using the user preferred option and displays the results and accuracy of that constructed tree.
   

ASSUMPTIONS:

1. Assuming training data and test data given are comapatible(meaning they both have same number of attributes).

2. code runs properly if user gives the command line arguments like file paths should proper as metioned above.






