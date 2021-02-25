frontend todo

# KNOWN BUGS

1. Add billing on user screen doesn't reset form or refresh table.
2. LEFT MODAL: When I click a user the request gets canceled and the site reloads?!?!
3. REPORTS COMPONENT IS FUCKED UP - THE route NO LONGER works
	- ie: ecommerce can have reports on a number of items, they all need their own


## DATA TABLE

1. If I force filters on a datatable via a VIEW card, those filters need to stay applied when I go to add additional filters.
	- Load a product, click on "CARTS" or "SUBSCRIPTIONS" then try to apply more filters. It will remove the product_id one.
		- Is the solution just fixing the criteria view to display all of the existing filters?