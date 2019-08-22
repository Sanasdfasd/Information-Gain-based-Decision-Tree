# Information Gain based Decision Tree

**Code Compiliation:**

In linux or ubuntu Environment 
use command g++ ID3_implementation.cpp 

In windows Environment open program in IDE and compile it.

**Code Execution:**

In ubuntu or linux Environment run the following commands to execute :
Command line inputs:
1. Training data file Path(like : c:\users\sandeep\train1.dat)
2. Testing Data file Path (Like : c:\users\sandeep\test1.dat)
3. pruning factor ( should be between 0 to 1 )

**./ID3_implementation.cpp train_data_file_path test_data_path prunefactor.**

To redirect output to a file, use the following command.

**./ID3_implementation.exe train_data_path test_data_path prunefactor > output_filename.txt**

In windows Environment after compling the program an new excutable will be generated.

Run the Executable using the following command:
ID3_implementation.exe train_data_path test_data_path prunefactor.

To redirect output to a file, use the following command.
**ID3_implementation.exe train_data_path test_data_path prunefactor > output_filename.txt**

**Output:**
 Pre pruned tree and the results.
 Post-pruned tree and the results.

**Assumptions:**

**1.** Assuming training data and test data given are comapatible(meaning they both have same number of attributes).

**2.** code runs properly if user gives the command line arguments like file paths and prune factor are properly as above mentioned.

**3.** pruning factor given as input to program should be between 0 and 1

**4.** pruning of nodes.
```  
//sample code explains the procedure that is followed in the process of pruning nodes.

   tp=nodes to be pruned.
   step_size=1; 
  while(tp>0)
  {
   iterate_decision_tree;
   if(node is leaf_node)
    {
      if(number of data instances that node covers < step_size && tp>0)
       {
          tp=tp-1,
          
       }
    }
          
    //After a full iteration through Decision tree if still the tp>0 then increase the stepsize.

  step_size=step_size+4 
  }
 
 ```
**Key Observation:** If a leaf node that covers relatively very less number of instances those instances can treated as error instances. 

**Accomplishments:**

Following the above procedure to prune the nodes.

**1.** After pruning the Tree Accuracy on test data is more than the pre pruned tree Accuracy on the same test data.

 This justifies that this method of pruning the nodes is acceptable.

**Note:** The Results of single run are saved in text file (Sample_run_results.txt) in the same folder

