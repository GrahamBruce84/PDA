### Testing task 1 code:

  Carry out static testing on the code below.  
  Read through the code.  Highlight any errors you can see without correcting them.

 
def func1 val                  - no brackets around parameter
  if val = 1
  return true                  - indentation is wrong
  else
  return false                 - indentation is wrong
  end
end
  
dif max a b                   - spelling mistake on def, should have brackets around parameters
  if a > b
      return a                 - indentation is wrong
  else
  b                            - indentation wrong
  end 
end 
end                            - Don't need this end
  
def looper                     - should have a parameter (i)
  for i in 1..10               - should have bracket round 1..10
  puts i 
  end
end
 
failures = 0 
 
if looper == 10                  
  puts "looper passed"
else
  puts "looper failed"
  failures = failures + 1
                                - no end
  
if func1(3) == failures         - calling on 3 as a parameter when it wasn't set in the method
  puts "func1(3) passed"
else
  puts "func1(3) failed"
  failures = failures + 1 
end 
 
  
if max(100,1) == 100            - shouldn't be == 100 we already set the parameters in the method
  puts "max(100,1) passed"
else
  puts "func1(3) failed"        - wrong sting
  failrues = failures + 1       - spelling mistake on failures
end

  
if failures                     - no parameters set
  puts "Test Failed"
else
  puts "Test Passed"
end


