# Add a new ruby definition

1. Go to https://github.com/rbenv/ruby-build and find your ruby version in the share folder. It'll look something like this:

`
install_package "ruby-1.8.6" "https://cache.ruby-lang.org/pub/ruby/1.8/ruby-1.8.6.tar.bz2#0fc6ad0b31d8ec3997db2a56a2ac1c235283a3607abb876300fc711b3f8e3dd7" warn_eol auto_tcltk standard
  install_package "rubygems-1.3.7" "https://rubygems.org/rubygems/rubygems-1.3.7.tgz#388b90ae6273f655507b10c8ba6bee9ea72e7d49c3e610025531cb8c3ba67c9d"
`

2. Download the file manually and verify it matches the sha256 digest given:

`> wget https://cache.ruby-lang.org/pub/ruby/1.8/ruby-1.8.6.tar.bz2
> openssl dgst -sha256 ruby-1.8.6.tar.bz2
SHA256(ruby-1.8.6.tar.bz2)= 0fc6ad0b31d8ec3997db2a56a2ac1c235283a3607abb876300fc711b3f8e3dd7
`

3. Copy and paste the file into the share folder of this repo. Commit & push.

That's it!

For more info on ruby-build, see: https://github.com/rbenv/ruby-build