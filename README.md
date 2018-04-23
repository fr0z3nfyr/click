
> **Click Tracking CakePHP Plugin**
> 
> Copyright (c) 2009 Matt Curry
> 
> www.PseudoCoder.com
> 
> http://github.com/fr0z3nfyr/click (Forked from: http://github.com/mcurry/click)
> 
> @author      Matt Curry <matt@pseudocoder.com>
> 
> @license     MIT


#### Instructions
1. Run the SQL in `/click/config/sql/clicks.sql` to create the DB table.
2. Include the helper in your AppController/Controller:
	```
	var $helpers = array('Click.click');
	```
3. Create your links using the helper (same syntax and options as `$html->link()`):
	```
	echo $click->link('PseudoCoder', 'http://pseudocoder.com');
	```
4. To view the click information download the [status plugin](https://github.com/fr0z3nfyr/status) (~~http://github.com/mcurry/status~~).  Once you have it setup add the click panels:
	```
	Configure::write('Status.panels', array('Click.latest', 'Click.most'));
	```
5. Go to `http://yourapp/status`
