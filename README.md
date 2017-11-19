# MsDocx [![Gem Version](https://badge.fury.io/rb/ms-docx.svg)](https://badge.fury.io/rb/ms-docx)

TODO: Delete this and the text above, and describe your gem

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'ms-docx'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install ms-docx

## Usage

```ruby
file_path = 'some_dir/'

# Read my_file.docx
doc = MsDocx::Document.open(file_path + 'my_file.docx')  

doc.each_paragraph do |par|
  # Change all paragraphs text to 'Test'
  par.text = 'Test'
end

# Save edited file
doc.save_file(file_path + 'new.docx')
```

TODO: Write usage instructions here

## Development

After checking out the repo, run `bin/setup` to install dependencies. Then, run `rake spec` to run the tests. You can also run `bin/console` for an interactive prompt that will allow you to experiment.

To install this gem onto your local machine, run `bundle exec rake install`. To release a new version, update the version number in `version.rb`, and then run `bundle exec rake release`, which will create a git tag for the version, push git commits and tags, and push the `.gem` file to [rubygems.org](https://rubygems.org).

## Contributing

Bug reports and pull requests are welcome on GitHub at https://github.com/[USERNAME]/ms-docx.
