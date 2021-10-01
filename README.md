# MidtermExamProblem6
Problem 6 Midterm

def max_val(t):
  '''t, tuple or list
  Each element of t is either an int, a tuple, or a list
  No tuple or list is empty
  Returns the maximum int in t or (recurively) in an element of t 
  '''
  def openItem(term):
    newList = []
    
    for item in term:
      if type(item) == int:
        newList.append(item)
        
     else;
       newList += openItem(item)
     return newList
     
     sortingList = openItem(t)
     maximum = sortingList[0]
     
     for item in sortingList:
     if maximum < item:
     maximum = item
     returm maximum
     
     print(max_val((5, (1,2), [[1],[2]])))
     print(max_val((5, (1,2), [[1],[9]])))
