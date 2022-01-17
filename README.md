- Added application partial links and new pages
- Style App with Bootstrap
- Manage User with Device gem:
    a) install devise
    b) add config.action_mailer.default_url_options = { host: "localhost", port: 3000 } to development.rb
    с) run rails g devise:views
    d) generate devise model 
    e) rails db:migrate
    f) edit header (add new routes)
    
- Associations (means that every user has his own friend list). A User has_many friend. Those friends belongs_to User. rails g migration add_user_id_to_friends user_id:integer. Then push the migration rails db:migrate. Let the system know when created a new friend and it belongs a user id

- More associations (fix 'edit' friend when u are not logged in (for this used before_action), create correct_user method, hide another user's friends list using condition)

- Style Modifications