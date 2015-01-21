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
    $('#Container').mixItUp(); // an instance now exists in the session memory
```

###Demoapp
open the folder demoapp to view an example of mixitup app.


####Issues you may find with turbolink
[mixitup-rails-turbolinks](http://www.asithadesilva.com/mixitup-rails-turbolinks/) and [github issues' page link](https://github.com/patrickkunka/mixitup/issues/111)

```javascript
$(function(){ // on first doc ready we instantiate mixitup
    $('#container').mixItUp(); // an instance now exists in the session memory
});
$(window).on('page:before-change', function(){ 
    $('#container').mixItUp('destroy'); // destroy the instance
});
$(window).on('page:load', function(){
    $('#container').mixItUp(); // We can now reinstantiate without being blocked
});
```

## Contributing

1. Fork it ( https://github.com/guinslym/mixitup_rails/fork )
2. Create your feature branch (`git checkout -b my-new-feature`)
3. Commit your changes (`git commit -am 'Add some feature'`)
4. Push to the branch (`git push origin my-new-feature`)
5. Create a new Pull Request
