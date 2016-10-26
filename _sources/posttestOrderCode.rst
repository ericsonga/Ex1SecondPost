.. qnum::
   :prefix: 1-3-
   :start: 1
   
.. |checkme| image:: Figures/checkMe.png
    :height: 20px
    :align: top
    :alt: check me
    
.. |start| image:: Figures/start.png
    :height: 24px
    :align: top
    :alt: start
    
.. |finish| image:: Figures/finishExam.png
    :height: 24px
    :align: top
    :alt: finishExam
    
.. |right| image:: Figures/rightArrow.png
    :height: 24px
    :align: top
    :alt: right arrow for next page
   
Post-test 2 Order Code Problem (Mixed Up Code)
--------------------------------------------------

Construct the function ``getAverage(nums,first,last)`` that takes a list of numbers, nums, and returns the average of the numbers between the first and last indices (inclusive). To do this first create a variable total and set its initial value to 0.  Then loop from the first index to the last index (inclusive) and get the current value at the index and add it to the total.  Check if the last index minus the first index plus one is greater than or equal to 1 and if so return the total divided by the last index minus the first index plus one.  Otherwise return 0 (to prevent a divide by 0).  

Examples
=========
   
For example ``getAverage([10,20,30],0,0)`` should return 10 and ``getAverage([10,20,30],1,3)`` should return 25.
    
Order Code Here
================

Click on the |start| button below when you are ready to try to order this code.  You will have up to 10 minutes to try to solve it.  Click on the |finish| button when you have solved this problem or wish to move on without solving it.

.. timed:: post_test2_avg_values_in_range
   :timelimit: 10
   :noresult:
   :nofeedback:
   :fullwidth:
   
   .. parsonsprob:: Post_Test2_Avg_Values_In_Range
      :order: 11,1,2,4,3,0,7,8,9,10,12,5,6
   
      The code below is mixed up and contains extra blocks that are not needed.  Drag the needed code from the left to the right and put them in order with the correct indention so that the code would work correctly.  
      -----
      # define function
      def getAverage(nums, first, last):
      =====
          # init total
          total = 0
      =====
          # init total
          total = 1 #paired
      =====
          # loop from first to last (inclusive)
          for index in range(first,last+1):
      ===== 
          # loop from first to last (inclusive)
          for index in range(first,last): #paired
      =====
              # get current at index
              current = nums[index]
      =====
              # get current at index
              current = index #paired
      =====
              # add current to total
              total = total + current
      =====
              # add current to total
              total = total + index #paired
      =====  
          # if at least one value
          if (last - first + 1) >= 1:
      =====
          # if at least one value
          if (last - first) >= 1: #paired
      =====
              # return average
              return total / (last - first + 1)
      =====
          # otherwise return 0
          return 0

When you are finished with this problem, or are ready to move on, click the |finish| button and then go to the next page by clicking the right arrow |right| near the bottom right of this page.    
    
   
  

      
               

           
           



    