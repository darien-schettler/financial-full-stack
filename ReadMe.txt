Flask-Vue Web Application for Financial Watchlists And Stripe Integration

####################################################################################


To begin you must first:


	1.  use npm/yarn to install dependencies within the Client folder.
		a.  yarn install
		b.  yarn run serve (launches local front-end server)

	
	2.  use the following commands to setup venv and dependencies within Server folder.
		a.  python -m venv env
		b.  env\bin\activate or env\scripts\activate
		c.  python -m pip install --upgrade pip
		d.  pip install -r requirements.txt
		e.  flask run (launches local back-end server)


####################################################################################

Things Done:
*	Basic CRUD application created utilizing FLASK & VUE
*	Use BOOTSTRAPVUE to make components and front-end simple
*	Hookup Stripe to allow for checkout web-flow

*	NOTE: There is a version on Gitlab working with Docker and Heroku which was created to explore pipeline deployment for a flask-vue CRUD SPA. PM for the link.

Things To Do:
*	Add client and server-side unit and integration tests.
*	Create a shopping cart so customers can purchase more than one book at a time.
*	Add Postgres to store the stocks/orders/etc.
*	Containerize Vue and Flask (and Postgres, if you add it) with Docker to simplify the development workflow.
*	Add profiles and let the main page be the 'watchlists' for individuals
*	Add images to the stocks (graphs maybe) and create a more robust product page.
*	Hook up the prices to a stock price api
*	Utilize ElasticSearch to find and add a stock to your 'Watchlist'
*	Capture emails and send email confirmations (review Sending Confirmation Emails with Flask, Redis Queue, and Amazon SES).
*	Deploy the client-side static files to AWS S3 and the server-side app to an EC2 instance.
*	Going into production? Think about the best way to update the Stripe keys so they are dynamic based on the environment.
*	Create a separate component for checking out.
*	Improve everything to do with checking out and verification
