- Added application partial links and new pages
- Style App with Bootstrap
- Manage User with Device gem:
    a) install devise
    b) add config.action_mailer.default_url_options = { host: "localhost", port: 3000 } to development.rb
    с) run rails g devise:views
    d) generate devise model 
    e) rails db:migrate
    f) edit header (add new routes)
-Associations (means that every user has his own friend list). A User has_many friend. Those friends belongs_to User. rails g migration add_user_id_to_friends user_id:integer

 