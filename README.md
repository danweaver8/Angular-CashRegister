## Angular-CashRegister

###Installing this demo
1. To try this out install node.js
2. Download this repo and run NPM install to install the required dependencies
3. This was written on a mac using visual studio code.
4. run `npm start` browse to http://localhost:8000/app/

###About
I took a small demo and expanded upon the layout and features and items. The initial demo helped me understand the factory and controller better and how this behavior was defined in the closure.

This is the first 1.0 version that I added additional features. The simplified version I originally got had items statically listed to add, no categories, no state tax, no way to take items off the receipt, the void transaction didn't work correctly, and there were no animations, and no ability to change a company.

###Modifications
1. I placed each category items in its own json file to load the items. The states were also stored in a json file. I next added the category dropdown which I populate statically for now. This was tricky at first until I got the deferred promise down.
2. I fixed the calculation adding and removing the employee discount.
3. I added the logic for voiding all transactions.
4. I added the logic to remove a specific item from the receipt based off of the product code. I had to modify the original logic because we needed a deep copy of the product to keep a unique code.
5. I changed the way the employee discount is added so it has the ability to be removed as well. You can only add 1 employee discount and will get a message if you try to add multiple.
6. I next added the receipt company, phone, and city which a user can change now. I had to create a service to allow the ability to update this from a different controller.
7. I added the ability to choose a state and apply the state tax.
8. The last thing I did was add some animations like when you choose a state from the dropdown, add items to a receipt, remove items from a receipt.

###Angular
This was a great exercise to learn angular in a deeper conceptual level than just following a tutorial where most of the work is done and handed to you. It helped me understand the factory and controller in greater detail. I also learned about creating a service and updating data provided between 2 controllers. I also got to apply my own animations and got to mess around with more CSS 3.0 elements and responsive designs.
