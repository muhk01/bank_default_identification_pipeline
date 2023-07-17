# bank_defaulter_identification_pipeline
Detecting a Bank defaulter using Apache Beam
Credit card skippers/defaulters:

--> Assign 1 point to customer for short payment, where a short payment means when customer fails to clear atleast 70% of its monthly spends.

--> Assign 1 point to customer where he has spent 100% of his max_limit but did not clear the full amount.

--> If for any month customer is meeting both the above conditions,assign 1 additional point.

--> Sum up all the points for a customer and output in file.




Loan file key points:

--> For Personal loan category, Bank does not accept short or late payments. If a person has not paid monthly installment then that month's entry won't be present in the file.

--> For Medical loan, Bank does accepts late payments but it should be the full amount. It is assumed that there is every month's data/record for Medical Loan.



Loan defaulters:

--> Medical Loan defaulters : If customer has made a total of 3 or more late payments.

--> Personal Loan defaulters : If customer has missed a total of 4 or more installments OR missed 2 consecutive installments.
