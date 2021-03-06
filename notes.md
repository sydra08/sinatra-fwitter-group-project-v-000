TO DO
[x] Set up directories and files

Models & Migrations
[x] Create User model
[x] Create Tweet model
[x] Users have username (string), email (string), password (string)
[x] A User has_many :tweets
[x] A User has_secure_password
[x] Tweets have content (string) and user_id (for association)
[x] A Tweet belongs_to :user
[x] Create Migrations

Controllers
[x] ApplicationController

Helper Methods
[x] #current_user => determine who the current user is based on the session id (?)
[x] #logged_in? => does the session[:id] exist for the current user?

Login
[x] enable sessions
[x] set session secret
[x] seed data?

Routes
[x] get '/' => homepage
[x] get '/tweets/new' => create a new tweet; tweet gets created and saved to db (cannot be blank!)
[x] get '/tweets' => show all tweets on twitter
[x] post '/tweets' => process new tweet request
[x] get '/tweets/:id' => view a single tweet; has link to edit tweet; option to delete tweet
[x] get '/tweets/:id/edit' => edit a single tweet
[x] patch '/tweets/:id' => process edit request
[x] delete '/tweets/:id/delete' => delete a tweet
[x] get '/signup' => form to create user - username, email and password
[x] post '/signup' => create user and persist db, after successful sign up the user is logged in
[x] get 'login' => display the login form
[x] post '/login' => process the login and add the user_id to the sessions hash
[x] get '/logout' => clear session

Views - remember that a user can only CRUD their own tweets!!!
[x] index.erb => homepage with links to login and signup pages
[x] create_tweet.erb => create a new tweet
[ ] edit_tweet.erb => edit a tweet
[x] show_tweet.erb => show a single tweet
[x] tweets.erb => show all tweets by a user (?)
[x] create_user.erb => user sign up form; only logged out users can see
[x] login.erb => user login page
[x] show.erb => show user information; logged out users can't see this
[x] layout.erb => html template for site

Misc
[ ] add flash messages
[ ] add lines between divs on Fwitter main feed page
[ ] clean up layout styling
[ ] review the login/logout issues
[ ] is there a reason you wouldn't use helper methods in the controllers? why !session[:user_id] vs logged_in?
[ ] create css stylesheet
[ ] can #current_user be used more in the controllers?
