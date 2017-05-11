mruby-io
========

`IO` class for mruby on ESP32

## Installation
Add the line below to your `build_config.rb`:

```ruby
  conf.gem :github => 'mruby-esp32/mruby-io', :branch => 'esp32'
```

## Implemented methods

### IO
 - http://doc.ruby-lang.org/ja/1.9.3/class/IO.html

| method                     | mruby-io | memo |
| -------------------------  | -------- | ---- |
| IO.binread                 |          |      |
| IO.binwrite                |          |      |
| IO.copy_stream             |          |      |
| IO.new, IO.for_fd, IO.open |  o  |     |
| IO.foreach                 |          |      |
| IO.pipe                    |    o     | not supported on ESP32 |
| IO.popen                   |    o     | not supported on ESP32 |
| IO.read                    |    o     |      |
| IO.readlines               |          |      |
| IO.select                  |    o     | not supported on ESP32 |
| IO.sysopen                 |    o     |      |
| IO.try_convert             |          |      |
| IO.write                   |          |      |
| IO#<<                      |          |      |
| IO#advise                  |          |      |
| IO#autoclose=              |          |      |
| IO#autoclose?              |          |      |
| IO#binmode                 |          |      |
| IO#binmode?                |          |      |
| IO#bytes                   |          | obsolete |
| IO#chars                   |          | obsolete |
| IO#clone, IO#dup           |          |      |
| IO#close                   |    o     |      |
| IO#close_on_exec=          |    o     |      |
| IO#close_on_exec?          |    o     |      |
| IO#close_read              |          |      |
| IO#close_write             |          |      |
| IO#closed?                 |    o     |      |
| IO#codepoints              |          | obsolete |
| IO#each_byte               |    o     |      |
| IO#each_char               |    o     |      |
| IO#each_codepoint          |          |      |
| IO#each_line               |    o     |      |
| IO#eof, IO#eof?            |    o     |      |
| IO#external_encoding       |          |      |
| IO#fcntl                   |          |      |
| IO#fdatasync               |          |      |
| IO#fileno, IO#to_i         |    o     |      |
| IO#flush                   |    o     |      |
| IO#fsync                   |          |      |
| IO#getbyte                 |          |      |
| IO#getc                    |    o     |      |
| IO#gets                    |    o     |      |
| IO#internal_encoding       |          |      |
| IO#ioctl                   |          |      |
| IO#isatty, IO#tty?         |    o     |      |
| IO#lineno                  |          |      |
| IO#lineno=                 |          |      |
| IO#lines                   |          | obsolete |
| IO#pid                     |    o     |      |
| IO#pos, IO#tell            |    o     |      |
| IO#pos=                    |    o     |      |
| IO#print                   |    o     |      |
| IO#printf                  |    o     |      |
| IO#putc                    |          |      |
| IO#puts                    |    o     |      |
| IO#read                    |    o     |      |
| IO#read_nonblock           |          |      |
| IO#readbyte                |          |      |
| IO#readchar                |    o     |      |
| IO#readline                |    o     |      |
| IO#readlines               |    o     |      |
| IO#readpartial             |          |      |
| IO#reopen                  |          |      |
| IO#rewind                  |          |      |
| IO#seek                    |    o     |      |
| IO#set_encoding            |          |      |
| IO#stat                    |          |      |
| IO#sync                    |    o     |      |
| IO#sync=                   |    o     |      |
| IO#sysread                 |    o     |      |
| IO#sysseek                 |    o     |      |
| IO#syswrite                |    o     |      |
| IO#to_io                   |          |      |
| IO#ungetbyte               |          |      |
| IO#ungetc                  |    o     |      |
| IO#write                   |    o     |      |
| IO#write_nonblock          |          |      |

## License

Copyright (c) 2013 Internet Initiative Japan Inc.

Permission is hereby granted, free of charge, to any person obtaining a 
copy of this software and associated documentation files (the "Software"), 
to deal in the Software without restriction, including without limitation 
the rights to use, copy, modify, merge, publish, distribute, sublicense, 
and/or sell copies of the Software, and to permit persons to whom the 
Software is furnished to do so, subject to the following conditions:

The above copyright notice and this permission notice shall be included in 
all copies or substantial portions of the Software.

THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR 
IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY, 
FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE 
AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER 
LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING 
FROM, OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER 
DEALINGS IN THE SOFTWARE.
