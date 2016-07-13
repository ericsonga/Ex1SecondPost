.. qnum::
   :prefix: 1-2-
   :start: 1

.. |runbutton| image:: Figures/run-button.png
    :height: 20px
    :align: top
    :alt: run button
   
.. |pass| image:: Figures/pass.png
    :height: 20px
    :align: top
    :alt: pass
    
.. |fail| image:: Figures/fail.png
    :height: 20px
    :align: top
    :alt: fail
    
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

               
Post-test 2 Fix Code Problem
-------------------------------
    
The code below is trying to calculate the average snowfall, but it contains errors.  It takes a list that contains the amount of snow for each day, collected by a meteorologist. Her equipment occasionally makes a mistake and reports a negative amount for that day.  Fix the code below to calculate the total snowfall by adding up all the non-negative values (including 0), also count the number of non-negative values, and return the average snowfall at the end.  Only return the average if there was at least one non-negative integer in the list, otherwise return 0.

Examples
=========

For example ``getAverageSnowfall([1, 2, -3, 3])`` should ignore the -3 and sum (1 + 2 + 3) which is 6 and then divide 6 by 3 (the number of values used in the sum) to return 2.  

Fix Code Here
==============

Fix the errors so that the hidden tests all print |pass| when you click the |runbutton| button. The error messages and test results are displayed below the code. 
               
Click on the |start| button below when you are ready to try to fix this code.  You will have up to 10 minutes to try to solve it.  Click on the |finish| button when you have solved this problem or wish to move on without solving it.

.. timed:: post_test2_snowfall_fix_timed
   :timelimit: 10
   :noresult:
   :nofeedback:
   :fullwidth:
    
   .. activecode:: Post_Test2_Snowfall_Fix
   
      def getAverageSnowfall(snow):

          # initialize the variables
          sum = -1
          num = 0
          
          # loop through the values in the list
          for value in Snow
		   
              # if the value is not negative
              if value >= 0:
   
              # add the value to the sum and increment the num
              sum = sum + value
              num = num + 1
  
          # if num is greater than 0
          if num >= 0:

              # calculate and print the average
              return sum / num
  
          # otherwise return 0
          return 0
          
      ====
          
      # code to test the getAverageSnowfall function        
      from unittest.gui import TestCaseGui
      
      class myTests(TestCaseGui):

          def testTarget(self):
              self.assertEqual(getAverageSnowfall([1, 2, -3, 3]), 2, "Test of getAverageSnowfall([1, 2, -3, 3])")
              self.assertEqual(getAverageSnowfall([-1, 2, 1, 3]), 2, "Test of getAverageSnowfall([-1, 2, 1, 3])")
              self.assertEqual(getAverageSnowfall([-1, -2, -1, -3]), 0, "Test of getAverageSnowfall([-1, -2, -1, -3])")
              self.assertEqual(getAverageSnowfall([-1, -2, 17, 13]), 15, "Test of getAverageSnowfall([-1, -2, 17, 13])")
              self.assertEqual(getAverageSnowfall([-1, 3, 17, 13, -2, 7]), 10, "Test of getAverageSnowfall([-1, 3, 17, 13, -2, 7])")
		   
      myTests().main()

When you are finished with this problem, or are ready to move on, click the |finish| button and then go to the next page by clicking the right arrow |right| near the bottom right of this page.    
