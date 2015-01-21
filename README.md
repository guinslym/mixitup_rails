# MixitupRails

Adding Mixitup in your rails app. MixItUp - A Filter & Sort Plugin  https://mixitup.kunkalabs.com

## Installation

Add this line to your application's Gemfile:

```ruby
gem 'mixitup_rails'
```

And then execute:

    $ bundle

Or install it yourself as:

    $ gem install mixitup_rails

## Usage

add in `app/assets/javascripts/application.js` after jquery (below jquery)

	//= require mixitup

```javascript
$(function(){ // on first doc ready we instantiate mixitup
    $('#Container').mixItUp(); // an instance now exists in the session memory
};
```


####Issues
[With turbolink](https://github.com/patrickkunka/mixitup/issues/111)

## Contributing

1. Fork it ( https://github.com/[my-github-username]/mixitup_rails/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
