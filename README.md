# JWT4B_Fork
Burp Extension to manipulate JWT forked from JWT4B @mvetsch with improved JWT recognition

This is a fork of https://github.com/mvetsch/JWT4B a very good BURP extension which enable to recognize, decode, and manipulate JWT.

The original JWT4B parser recognize JWT based on parameter format in BODY request with specific keywords as name (e.g. in the format JWT=..&anotherparameter=..).

This fork add JWT recognition pattern in BODY so that it can recognize more JWT during the parsing phase. In particular it recognizes JWT sent within JSON objects, or in a parameter format but without keywords. It also recognize JWT which are send as a single string (provided there is a blank at the beginning and at the end of the JWT).
