# Sports_Refrence-Internship

# Code Explanation

I have used python as my language of choice.

<ul>
  <li> I first import the modules that will be requiored for reading and manipulating the json file</li>
  <li> Then i read the json file using thr json module.</li>
  <li> Now the json file is in the form of dictionary, and thus i can iterate through it. Now the json file is in the structure as { Mainkey:{subkey:{"W":,"L":}} . thus i use two for loops one loop to interate through thr Mainkey and other though the subkey.</li>
  <li>Now i understood that there was no need for "L" in the subkey dictionary. Beacause in the output table we only need to display the wins. To do that i iterate through the dictionary and pop out the "L" from the subkey dictionary</li>
<li>TO have proper structure i empty the dictionay with W and L and just enter the numerical value of W. This gives me the final desired structure to convert it into the required table format</li>
  <li>I use pandas from_dict to conver the dictionary into dataframe and use orient="index".This helps me notifying that the Mainkeys should be used has Index column names.I also fill the NAN values with "--" to have the deseried table </li>
</ul>
