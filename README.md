### Bunny
---
https://github.com/ruby-amqp/bunny

```
gem install bunny
gem "bunny", ">= 2.12.0"

```

```ruby
require "bunny"
conn = Bunny.new
conn.start
q = conn.create_channel
q = ch.queue("test1")
q.publish("Hello")
delivery_info, metadata, payload = q.pop
puts "This si the message: #{payload}"
conn.stop

```

```
```
