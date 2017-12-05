# Problem without solution
In  case I use list<int> and list<string>
  in the same function preview string shows correct values but the expanding section will 
  cast the type of the list to the first type declared in this scope.
  For instance 
  
  list<int> lint; </nl>
   //... fill some vals 1 2 3 </nl>
  list<string> listr;  </nl>
  //... fill some vals "1" "2" "3" </nl>    
    
  debugger will show 
  lint 1,2,3 .... </nl>
    1 </nl>   
    2 </nl>   
    3 </nl>
    xxx </nl>    
    1 </nl>   
    2 </nl>    
    3</nl>    
    xx</nl>    
    ...</nl>
    
  listr "1","2","3" ... </nl>
    some number </nl>
    some number </nl>
    some number </nl>
    xxx </nl>
    some number</nl>
    some number</nl>
    some number</nl>
    
Same for map<></nl>

Still dont have solution for this !!!

  
# stlport_natvis
stlport version 5.2
VS2012

# general info
https://msdn.microsoft.com/en-us/library/jj620914(v=vs.110).aspx#BKMK_LinkedListItems_expansion
https://code.msdn.microsoft.com/windowsdesktop/Writing-type-visualizers-2eae77a2/view/Discussions

# to install:
copy.bat

# To Do
Adapt the autoexp.dat stlport visualisers to natvis format.
File per container approach


