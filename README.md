# Problem without solution
In  case I use list<int> and list<string>
  in the same function preview string shows correct values but the expanding section will 
  cast the type of the list to the first type declared in this scope. </br>
  For instance </br>
  
  list<int> lint; </br>
   //... fill some vals 1 2 3 </br>
  list<string> listr;  </br>
  //... fill some vals "1" "2" "3" </br>    
    
  debugger will show </br>
  lint 1,2,3 .... </br>
    1             </br>
    2             </br>
    3             </br>
    xxx           </br>
    1             </br>
    2             </br>
    3             </br>
    xx            </br>
    ...           </br>
    
  listr "1","2","3" ... </br>
    some number         </br>
    some number         </br>
    some number         </br>
    xxx                 </br>
    some number         </br>
    some number         </br>
    some number         </br>
    ...
    
Same for map<>          </br>

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


