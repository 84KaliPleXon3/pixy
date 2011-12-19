# Pixy

[![Build Status](https://secure.travis-ci.org/NARKOZ/pixy.png)](http://travis-ci.org/NARKOZ/pixy)

Pixy is an API wrapper for Pixiv url shortener - [p.tl](http://p.tl/)

## Installation

```ruby
gem 'pixy'
# gem install pixy
```

## Usage

```ruby
Pixy.shorten!(API_KEY, 'https://github.com/narkoz/pixy')
# => "http://p.tl/Us9R"

pixy = Pixy.shorten(API_KEY, 'https://github.com/narkoz/pixy')
# => #<Pixy::Shorten:0x0000010201bde8 @status="ok", @long_url="https://github.com/narkoz/pixy", @short_url="http://p.tl/Us9R", @counter=20>

pixy.status
# => "ok"

pixy.long_url
# => "https://github.com/narkoz/pixy"

pixy.short_url
# => "http://p.tl/Us9R"

pixy.counter
# => 20
```

## Copyright

Copyright (c) 2011 Nihad Abbasov    
BSD License.
