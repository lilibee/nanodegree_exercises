# nanodegree_exercises
#i am dooing a udacity data analyst nanodegree this is code i need to share

#exercise 16 lesson 4
def reverse_names(name):
    name = name.split()
    name_new = name[1] + ',' + name[0]
    return name_new    
'''
    Fill in this function to return a new series where each name
    in the input series has been transformed from the format
    "Firstname Lastname" to "Lastname, FirstName".
    
    Try to use the Pandas apply() function rather than a loop.
'''
 
reverse_names = names.apply(reverse_names)

'''
here was an error running your code:

Traceback (most recent call last):
  File "vm_main.py", line 33, in <module>
    import main
  File "/tmp/vmuser_vlyqylmtnd/main.py", line 2, in <module>
    import aiMain
  File "/tmp/vmuser_vlyqylmtnd/aiMain.py", line 94, in <module>
    correct, comment, feedback = get_feedback()
  File "/tmp/vmuser_vlyqylmtnd/aiMain.py", line 87, in get_feedback
    test_correct, test_comment = test_case.grade(pandas_series_apply)
  File "/tmp/vmuser_vlyqylmtnd/aiMain.py", line 44, in grade
    student_result = student_lib.reverse_names(self.names)
TypeError: 'Series' object is not callable
'''
  
