Steps to make this repository work
1. Initialize a new bench using 'bennch init --frappe-branch <branch-name> <bench-name>'. For example: bench init --frappe-branch develop ascra
  This will clone and install frappe app from the specified branch
2. Go to the bench directory created, 'cd ascra'
3. Create a new site using 'bench new-site <site-name>' For example: bench new-site ascra_tech
4. Now get the ERPNext app using 'bench get-app [--branch <branch>] <APP_REMOTE_URL>'
5. Now install your ERPNext app on the site created in step 3 using 'bench --site <site-name> install-app <app-name>'
6. Now get this app using 'bench get-app [--branch <branch>] <APP_REMOTE_URL>'
7. Now install this app on the site created in step 3 using 'bench --site <site-name> install-app <app-name>'
8. Try running a 'bench start', It should start a normal bench. Once its started, the site can be accessed on any browser.
9. Now in a new terminal, run 'bench migrate', keep the bench started as its required for migrate to run
10. Go to the site/desk, login to the desk
11. Create a new Company, a new Customer, a new Item, Pricing List for Item, Item Price fro item
12. You might need to update a Fiscal year, Create a Bank Account, Account Type, Account, Address for Customer and Company
13. Now, try creating a Sales Invoice with all the details for a customer, using the item created.
14. Once all details are filled, Submit the Invoice.
15. Once Submitted, print the Invoice using the print button on top, Select the 'Invoice' print format from the 'Select Print Format' dropdown.
16. Voila!