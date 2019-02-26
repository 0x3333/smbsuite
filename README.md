# smbsuite
A suite of Apps to easily manage `samba` file server from the Web.

## Motivation
I quite often implement a `samba` file server using `Share` security, this is the easiest way to implement `samba`, but you have to manage it all by hand, and this can be quite a pain.

The idea of this project is to create a foundation to build simple apps to manage this tasks using a Web browser. Initially I'll implement `smbpasswd` for users and `ACL` permissions management. But new Issues/PR can be created to ask/implement new features.

## Plan

I don't know yet how these "apps" will be implemented, but I will create a RESTful server using `Go-lang`.
Some small binaries will be created to make a bridge between the REST API and the samba executables,
like `smbpasswd`, 'getfacl', 'setfacl', to sanitize and validate the input to these programs.

The UI will be implemented probably using `Vue.js` and Bootstrap v4.

## License

    MIT License
    
    Copyright (c) 2019 Tercio Gaudencio Filho
    
    Permission is hereby granted, free of charge, to any person obtaining a copy
    of this software and associated documentation files (the "Software"), to deal
    in the Software without restriction, including without limitation the rights
    to use, copy, modify, merge, publish, distribute, sublicense, and/or sell
    copies of the Software, and to permit persons to whom the Software is
    furnished to do so, subject to the following conditions:
    
    The above copyright notice and this permission notice shall be included in all
    copies or substantial portions of the Software.
    
    THE SOFTWARE IS PROVIDED "AS IS", WITHOUT WARRANTY OF ANY KIND, EXPRESS OR
    IMPLIED, INCLUDING BUT NOT LIMITED TO THE WARRANTIES OF MERCHANTABILITY,
    FITNESS FOR A PARTICULAR PURPOSE AND NONINFRINGEMENT. IN NO EVENT SHALL THE
    AUTHORS OR COPYRIGHT HOLDERS BE LIABLE FOR ANY CLAIM, DAMAGES OR OTHER
    LIABILITY, WHETHER IN AN ACTION OF CONTRACT, TORT OR OTHERWISE, ARISING FROM,
    OUT OF OR IN CONNECTION WITH THE SOFTWARE OR THE USE OR OTHER DEALINGS IN THE
    SOFTWARE.
