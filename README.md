# Reddit の Cloneを作る

■参考
https://medium.com/@deallen7/how-to-build-a-reddit-like-site-with-ruby-on-rails-7b6cd106463d

■acts_as_votable
https://github.com/ryanto/acts_as_votable
https://qiita.com/YutoYasunaga/items/7ba03180ab3d2d8473b8#_reference-2ef5a487ebda2bf1f058

■Simple Form
https://github.com/plataformatec/simple_form
https://qiita.com/Inp/items/4f72918c2fba0d3a8809

■record_tag_helper
https://github.com/rails/record_tag_helper

■Deviseでpassword confirmationしか表示されない
http://azuuun-memorandum.hatenablog.com/entry/2017/10/16/184723
`app/views/devise/registrations/new.html.erb`を修正

```
<div class="form-group">
      <%= f.label :password_confirmation %>
      <%= f.password_confirmation_field :password, class: "form-control", required: true %>
</div>
↓
<div class="form-group">
      <%= f.label :password %>
      <%= f.password_field :password, class: "form-control", required: true %>
</div>
```
■Form_forメソッド
https://qiita.com/Momozono/items/319bc503e6a5f0963ab9
